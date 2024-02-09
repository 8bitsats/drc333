Introduction to DRC333 Standard

I propose a pioneering standard for dynamic and interactive art collections that leverage recursive inscriptions to reduce the cost of imagery inscription on Dogecoin via the Doginals protocol significantly.

Drawing inspiration from the foundational BRC69 and BRC333 standards by luminex and Owinals, my standard introduces on-chain functionalities like pre-mint and on-chain reveals. This is facilitated through the Doginals explorer, enabling image drawing without the necessity for inscribing trait images or undertaking additional actions.

Currently, this standard is optimized for pixel-based collections, with plans to expand support to vector-based collections in the future.

Context

The rising popularity of the Doginals protocol and the subsequent surge in fungible token inscriptions, particularly DRC-20, have led to increased demand for blockspace on the Dogecoin network. This surge has resulted in unusually high fees, adversely affecting Doginals art creators and collectors due to the larger size of image inscriptions compared to text inscriptions used for trading fungible tokens. 

Such conditions have compelled creators of Doginal collections to postpone or abandon their projects, discouraging new creators from venturing into the Dogecoin ecosystem. To foster continued innovation within Dogecoin blockchain collections, I introduce a novel approach for launching pixel art Doginal collections.As the Doginals protocol gains traction, fungible token inscriptions (most notably DRC-20) have greatly increased the demand for blockspace on the Dogecoin network. 

This has led to abnormally high fees, which disproportionately affect Doginals art creators and collectors, 
because image inscriptions are larger than text inscriptions such as those used to buy and sell fungible tokens. 
This has forced Doginal collection creators to delay or cancel plans for Doginals collections, 
and discourages creators from entering the Dogecoin space. 

In order to continue encouraging creators to launch innovative collections on the Dogecoin blockchain, 
we propose a new approach for launching pixel art Doginal collections.

The Idea

I introduce a new standard aimed at launching non-fungible Doginals collections. This standard employs recursion to decouple logic from the mint script, potentially reducing block space requirements by 50% to 90%+, depending on the collection size and network fees.

I propose a new standard for launching non-fungible Doginals collections. 
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

The implementation process involves three primary steps:

	1.	Inscribe the DRC333 Collection Deployment JSON: This step involves inscribing a JSON text that outlines general information about the collection along with a color palette array for each trait.
	2.	Inscribe the DRC333 Collection Compiler JavaScript: This involves inscribing a JavaScript that serves as the compiler for the collection, facilitating the rendering process based on the traits and their coordinates.
	3.	Inscribe the DRC333 Asset with the Mint Operation: Finally, the asset itself is inscribed with the mint operation, completing the creation process.

This entire process can be executed without relying on an external indexer, provided that collection creators publish the official list of color palettes and trait coordinates for their collections as currently required. Furthermore, images will be automatically rendered on all front-end interfaces that support Recursive Inscriptions, streamlining the process by eliminating the need for additional steps.

Operations

Deploy DRC333

The Deploy operation involves a JSON/Text inscription that encompasses general collection information and a detailed array of color palettes for each trait. This inscription acts as both a reference and the definitive source for the trait’s color palette. Optionally, it can include coordinates for the traits, delineating the design’s shapes and enabling the compiler to automatically render these traits on the front-end. For broader applicability, creators may choose to inscribe the coordinates in a separate JSON or JavaScript file, facilitating their use in various contexts.
DRC333

The Deploy operation is a JSON/Text inscription that contains general information about the collection and an array of color palettes for each trait. 
The deploy inscription serves as the reference and the definitive source for the color palette of traits.

The deploy inscription can optionally include the coordinates of the traits, 
which describe the shapes in the design and are used by the compiler to automatically render the traits on the front-end. 
If the creator wants to make it easy for others to use the coordinates in other contexts, they can inscribe the coordinates in a separate JSON or JavaScript inscription.
