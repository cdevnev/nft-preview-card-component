# nft-preview-card-component

The goal of this project was to replicate the preview card layout as provided, including some styled hover states on select elements.

Problems I expected: 
- Figuring out how to create the image overlay for the hover state
- Replicating the centering solution I used in a previous project to align everything on the page
- Properly making use of the responsive media queries I avoided last time around

Problems I didn't expect:
- Working through positioning issues within my (flex) containers 

I approached this project similarly to the last since they shared so many design elements. The wrapper and container solution to center vertically (via display:table and display:table-cell) worked without issue, but I struggled to align the flex'd icons/svgs and their associated text elements until I realized I needed to display:table-cell those as well. 

Instead of lazily avoiding the media queries, this time I opted to use them toward the end of the project to slightly adjust the scaling of fonts (the design docs seemed to indicate a change in size, but hard to guesstimate via JPG) and slightly scale the card width as well. This took some tinkering to get it working how I liked, and I ended up doing a lot of research on rem units as they relate to media queries for font scaling. More research needed there.

The hover elements came last and presented some trouble. Working with yet another wrapper allowed me to position the overlay and icon easier, but I still needed to figure out how to use the conventional transform: translate() to center, as the table-cell solution wouldn't work here. The actual hover effect was not too difficult to replicate but it took some research to figure out the wrapper was needed and the markup/layout that was required to get it to all work together. 

I also did a _better_ job of making commits during the project, but I need to adjust my workflow. I tend to jump around a lot and so my commits have lots of changes across the document instead of targeted changes to specific elements/features. I'm not sure if I can do anything about that until I start branching the project and focusing on individual features/functions instead of the whole-document process I've been doing. I imagine a lot of that will come with experience, so ... on to the next project!

Thank you for reading and as always, please comment with any feedback!