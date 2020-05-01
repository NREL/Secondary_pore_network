# Secondary pore network design optimization analytical diffusion model for lithium ion battery
Repository of Secondary Pore Network (SPN) analytical model applied to battery electrodes

## Auhtors
This model has been published along with the article below. Please quote it if distributing the model and/or results obtained with it.

F. L. E. Usseglio-Viretta<sup>a</sup>, W. Mai<sup>a</sup>, A. Colclasure<sup>a</sup>, M. Doeff<sup>b</sup>, Eongyu Yi<sup>b</sup>, and K. Smith<sup>a</sup>, Enabling Fast Charging of Lithium Ion Battery Through Secondary/dual Pore Network: Part I – analytical diffusion model, Electrochemica Acta, 342 (2020) 136034.\
<sup>a</sup> Transportation and Hydrogen Systems Center, National Renewable Energy Laboratory, Golden, Colorado 80401, USA\
<sup>b</sup> Energy Storage & Distributed Resources Division, Lawrence Berkeley National Laboratory, Berkeley, CA 94720, USA\
DOI: https://doi.org/10.1016/j.electacta.2020.136034

If you have questions or comments, please send message to: Francois.UsseglioViretta@nrel.gov

The model homepage is:\
Secondary pore network design optimization analytical diffusion model for lithium ion battery. https://www.nrel.gov/transportation/electrode_secondaryporenetwork.html.\
Tutorial video is available at https://www.youtube.com/watch?v=5RxZEIxKzzQ&feature=emb_logo\

## Presentation

Fast ion transport along the electrode thickness is required for Lithium ion battery (LIB) to sustain continuous high-rate discharge or charge currents, which is a desired feature for the fast charging of electric vehicle batteries. Advance in LIB electrode manufacturing allows to control, to a certain extent, the electrode microstructure architecture in order to improve the macroscopic performances of these devices. For instance, several groups have experimentally tested architectures tailored specifically to increase the through plane ionic diffusion in regards for fast charge application by adding channels or groove-like large pores oriented along the electrode thickness. These voids do not replace the existing pores of the electrode microstructure but consist in a second, coarser, pore network, called the secondary pore network (SPN).

The model quantifies the impact of SPN on ionic diffusion with a composite electrode through a simple analytical approach, considering various pore channel geometries and comparing to standard electrodes with identical gravimetric and identical volumetric specific theoretical capacity. The goal is to find optimal SPN design parameters according to three optimization objectives aiming to balance the improved overall through-plane, thanks to the coarse aligned channels, and the degraded in-plane diffusion, due to the porous matrix densification required to maintain gravimetric and volumetric specific theoretical capacity.

The analytical model must be considered as a pre-screening tool to quickly investigate large design space, that can be refined later with more complex electrochemical CPU-expensive numerical models.

## Description

The model analytically calculates effective diffusion coefficient, tortuosity factors, and characteristic diffusion time of a composite electrode considering a secondary pore network on top of the pre-existing microstructure finer pore network. Effective diffusion coefficients are deduced using parallel and series analytical law. Parameters considered are the electrode total porosity, the ratio of carbon black additives, the tortuosity factor coefficients including its anisotropy, the SPN channel geometry (rectangular or cylindrical), the SPN volume fraction and width dimensions, the ratio between SPN channel width and electrode thickness, the dimension of an (optional) pad layer without SPN at the back of the electrode, and the method of comparison (keeping thickness identical between the structured and reference electrode to preserve both gravimetric and volumetric specific theoretical capacity, or relaxing the thickness constraint). Parameters can be entered using a unique value or bounded values. In the latter case, the model will be run multiple times between these bounds allowing investigating large design space and results are shown using two-dimensional map. 

Optimal design parameter are chosen according to three different, non equivalent, but both aiming to balance through-plane with in-plane diffusion, optimization objectives. The first consists in maximizing the product of the electrode through-plane diffusion gain with the the porous matrix in-plane diffusion gain. The second aims to enforce diffusion coefficient isotropy, while the last one targets diffusion characteristic time isotropy.

Model runs within the MATLAB live editor environment: code is hidden (but accessible if user wish to see it) leaving visible only formatted text, equations, pictures, and results. Documentation is included directly in the live editor environment. Parameter inputs are entered with a graphic user interface (edit field, slider, check box, push button, and drop down buttons). Results are generated in figures, in the MATLAB window but can also be automatically saved in png and fig format in a user-defined folder.

No external inputs are required. A tutorial video is attached.

# Note:
The model file uses the term 'reference electrode' while the article uses the term 'baseline electrode' to speak of the unstructured electrode.