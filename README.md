# slice2mesh: a Direct Mesher of Sliced Data for the Simulation of AM Processes

**[Marco Livesu](http://pers.ge.imati.cnr.it/livesu/), Daniela Cabiddu, [Marco Attene](http://pers.ge.imati.cnr.it/attene/PersonalPage/attene.html)**

**CNR IMATI Genoa, Italy**

Accurately simulating Additive Manufacturing (AM) processes is useful to predict printing failures and test 3D printing without wasting precious resources, both in terms of time ad material. In AM the object to be fabricated is first cut into a set of slices aligned with the build direction, and then printed, depositing or solidifying material one layer on top of the other. To guarantee accurate simulations, it is therefore necessary to encode the temporal evolution of the shape to be printed within the simulation domain. We introduce slice2mesh, to the best of our knowledge the first software capable of turning a sliced object directly into a volumetric mesh. Our tool inputs a set of slices and produces a tetrahedral mesh that endows each slice in its connectivity. An accurate representation of the simulation domain at any time during the print can therefore be easily obtained by filtering out the slices yet to be processed. slice2mesh also features a flexible mesh generation system for external supports, and allows the user to trade accuracy for simplicity by producing approximate simulation domains obtained by filtering the object in slice space.