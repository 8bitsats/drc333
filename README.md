DRC333
I propose a new standard for dynamic and interactive art collections that utilize recursive inscriptions to lower the cost of inscribing imagery on Dogecoin using the Doginals protocol. 

Inspired by the original BRC69 and BRC333 from luminex and Owinals, 
this standard supports on-chain features, such as pre-mint and on-chain reveals. 
This is achieved by drawing the image on the Doginals explorer, without the need for inscribing trait images or additional action.

Currently, the standard supports pixel-based collections. We anticipate supporting vector-based collections in the future.


Context

As the Doginals protocol gains traction, fungible token inscriptions (most notably DRC-20) have greatly increased the demand for blockspace on the Dogecoin network. 
This has led to abnormally high fees, which disproportionately affect Doginals art creators and collectors, 
because image inscriptions are larger than text inscriptions such as those used to buy and sell fungible tokens. 
This has forced Doginal collection creators to delay or cancel plans for Doginals collections, 
and discourages creators from entering the Dogecoin space. 
In order to continue encouraging creators to launch innovative collections on the Dogecoin blockchain, 
we propose a new approach for launching pixel art Doginal collections.

Idea
We propose a new standard for launching non-fungible Doginals collections. 
This standard leverages recursion to separate the logic from the mint script, 
providing a 50% to 90%+ reduction of block space, depending on the size of the collection and network fees. 

The process involves three steps:

1. Inscribe the DRC333 collection deployment JSON
2. Inscribe the DRC333 collection compiler JavaScript
3. Inscribe the DRC333 asset with the mint operation

All these processes can be conducted without an external indexer,
as long as the collection creators release the official list of color palettes and trait coordinates for their collections,
as currently required. Moreover, the images will be automatically rendered on all front-end interfaces that implement Recursive Inscriptions,
eliminating the need for additional steps.

Operations
Deploy DRC333
The Deploy operation is a JSON/Text inscription that contains general information about the collection and an array of color palettes for each trait. 
The deploy inscription serves as the reference and the definitive source for the color palette of traits.

The deploy inscription can optionally include the coordinates of the traits, 
which describe the shapes in the design and are used by the compiler to automatically render the traits on the front-end. 
If the creator wants to make it easy for others to use the coordinates in other contexts, they can inscribe the coordinates in a separate JSON or JavaScript inscription.

This revised text aligns with the context of Dogecoin and the Doginals protocol, replacing Bitcoin and Ordinals references accordingly.

