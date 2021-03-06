## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/shiangfang/shiangfang.github.io/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/shiangfang/shiangfang.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact


Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.


## CS 205 Project

### Motivation

Conventional bulk solids are made of three-dimensional crystals with strong chemical bonding in between atomic constituents. Ever since the [discover of graphene](https://www.nobelprize.org/nobel_prizes/physics/laureates/2010/press.html), there are intense reserach investigations on the layered materials. These are the materials with strong chemical bonding between the atoms in the same sheet and weaker van der Waals interactions between the neighboring sheets. Because of the nature of the bonding, the sheets of atoms can be exfoliated using mechanical method with tapes. Over the years, the members of the 2D materials are constantly growing with new types of layers that can be exfoliated or fabricated. They can host a variety range of physical properties as well. For example, some layers can be magnetic or superconducting. There are great implications for the applications using these layered materials in the industry or fundamental research.

Because they are sheets of materials, one might be interested in stacking different layers together to form a stack like a sandwich and hope to engineer the stack with the desired properties by combining them properly. There are many control knobs in forming the stack, for example, what types of layers to be used, and what is the twist angle in stacking and the geometry. Though it is exciting to imagine the possibility to use these layered materials, theoretically it is extremely challenging to simulate the layer stacks and give insights for the experimental parameters to be tested. 

To understand the difficulty, we can first look at the system from the geometry point of view. Moire pattern is the interference pattern created when two similar images are overlapping with each other. It can be observed in daily life such as the photography [maybe with an example here?]. The overlap between two images would create a long-wavelength varying pattern in the combined image. The scale of this long-wavelength variation is determined by the degree of the mismatch between layers. The smaller the mismatch is, the larger the length scale is for the spatial variations. The similar phenomena would occur for atomic crystals as well and the two-dimentional geometry for the layered materials are perfect to illustrate this Moire pattern physics. 

For the example of the graphene, if we have two sheets on top of each other and with about 1 degree twist angle, the Moire pattern would have a length scale about 13 nanometer and it has a triangle lattice structure. This super-structure, the large length scale atomic variation usually contains over 10,000 atoms and this causes tremendous challenges for numerical simulations for these twisted bilayer system.

However, if we zoom in on these twisted bilayer system, we can see locally they resemble the perfect aligned crystal with the relative shift between layers that depends on the location in the super-structure. In other words, this large scale sctructure can be viewed as made of patching of various configurations of aligned crystals that has much smaller system size. Intuitively one can imagine that by studying the smaller structure of the crystal and their electronic properties and how they depend on the crystal layer shift, we can infer or construct the corresponding patched super-structure and reduce the computational resources that are needed to perform the simulation. This is in line with the multi-scale simulations. The DFT+Wannier technique mentioned above provides the necessary toolset for performing such task. First, for the smaller periodic crystal, the DFT+Wannier method is used to extract the orbital information, their coupling strength and the electronic properties, and how they vary with interlayer shift. After the basic ingredients for the modeling are obtained, we can patch these local models to form the global model for the super-structure and perform the electronic simulations. 

Overcoming this theoretical challenge to simulate the van der Waals heterostructure and twisted structure is crucial to advance the current semiconductor industry and fundamental physics research. One of the recent excitement is the discovery of superconductivity in the twisted bilayer graphene at "magic angle" (about one degree): [Surprise graphene discovery could unlock secrets of superconductivity](https://www.nature.com/articles/d41586-018-02773-w). For each individual graphene monolayer, superconductivity is not present unless it is in proximity with other convention superconductors. The superconductivity displayed this way is not intrinsic to the graphene layers. However, what is really interesting and surprising is that when two layers of graphene are stacked with a small magic twist angle, the bilayer heterostructure become superconducting at about 1 Kelvin and it is intrinsic transport property. The origin of this suerpconductivity phase is still under intense debte and subject of current research topic now. However, it is related to the peculiar electronic band structure in the twisted bilayer graphene. At this magic angle, a set of nearly flat bands are present and these bands with low dispersion and quenched kinetic energy are usually beneficial for inducing stronger interaction effects (from electron-electron mutual interaction). Ths superconductivity is expected to originate from the enhanced interaction effects.

Looking forward to the research with these van der Waals layer stacking, there are many open questions. How could we determine or engineer the proper layer structure and what is the geometry that we should create in order to manipulate the electronic properties to what we desire, how to optimize the combinations, and what should we be expecting for the new physics to emerge. These are extremely challenging and exciting to explore, but the efficient numerical approach and toolset are necessary to perform these simulations. One strong benefit of creating the database and having very efficient ways of querying the data entries for the related crystal types and geometry is extremely valuable to advance the theoretical approach. With the growing number of two-dimentional layered materials and various forms, our database can also be extended to many types and symmetries. One can proceed with the truly ab-initio simulations of these layer stacks, or derive the corresponding low-energy expansions and various handy models to describe them.



### Workstation details:






### DFT+Wannier method:
DFT is the state of the art microscopic quantum mechanical simulation for materials, however it is not straightforward to derive the physics picture from the massive information output from running a DFT simulation. Intuitively what Wannier transformation does is to interpret the DFT calculation results in terms of localized Wannier function basis. These can be thought of as the chemical atomic orbitals that participate in the bonding and hybridization of the electrons. The first step is to apply this DFT+Wannier method to various types of two-dimentional 



### future looking for generalizations











