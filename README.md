# ESMART-HW-LIB-PUB
ESMART-HW-LIB-PUB is the public E-SMART hardware part library. It is created for the purpose of holding the hardware parts designed by Laurence Deschênes-Villeneuve and part of his open source library [REEKILIB](https://gitlab.com/real-ee/lib/reekilib). The purpose of this repository is to act as a save point for the part used in E-SMART propriatary hardware designs. Since REEKILIB is covered by the [GPL-v3.0][license_GPL], these hardware parts must be available for public use free of charge. However, anyone who wishes to use, fork or copy the parts and models must respect the GPL-v3.0 license.

**No support, updates, releases or modifications will be made to this repository from the original release.**

# REEKiLib explained

This is a parts library for [KiCAD][kicad_link] from [RealEE][realee_link] containing schematic symbols, PCB footprints, 3D models, simulation model, templates and others utils for HW design.  
This [repo][reekilib_link] is not intended to be added as a git submodule as it is quite heavy, rather you should install it locally on your workstation.

## Compatibility

This library is mainly aimed at the [stable][kicad_install_link] version (currently 8) but may be compatible with [previous][kicad_install_link] (6,7) and [newer][kicad_install_link] (9+) versions.

## Organization

- _[3dmodel][3dmodel_folder]_: 3D models used in the footprints
- _[footprint][footprint_folder]_: Standard and custom PCB footprints grouped by type inside subfolder
- _[simmodel][simmodel_folder]_: Simulation (SPICE & IBIS) parts model _(limited to publicly available models)
- _[symbol][symbol_folder]_: Schematic symbol available in this lib

# How to use

1. clone the [repo][reekilib_link] to a local folder accessible to KiCAD
2. create an [environment variable][kicad_doc_path_link] inside KiCAD named `ESMART-HW-LIB-PUB` pointing to the root folder of the repo
3. [install][kicad_doc_libinstall_link] the necessary symbol lib from the folder [symbol][symbol_folder]
4. [install][kicad_doc_libinstall_link] the necessary footprint lib from the folder [footprint][footprint_folder]


<!-- links -->

[realee_link]: https://www.realee.tech/
[reekilib_link]: https://gitlab.com/real-ee/public/reekilib
[kicad_link]: https://www.kicad.org/
[freecad_link]: https://www.freecadweb.org/
[repo_link]: https://github.com/Esmartdriver/esmart-hw-lib-pub

<!-- doc links -->

[kicad_doc_link]: https://docs.kicad.org/8.0/en/
[kicad_doc_path_link]: https://docs.kicad.org/8.0/en/kicad/kicad.html#paths_configuration
[kicad_doc_libinstall_link]: https://docs.kicad.org/8.0/en/kicad/kicad.html#libraries-configuration
[kibot_doc_link]: https://kibot.readthedocs.io/en/master/

<!-- files -->

[license_GPL]: ./GPL-license-copy

<!-- folder -->

[doc_folder]: doc/
[footprint_folder]: footprint/
[3dmodel_folder]: 3dmodel/
[simmodel_folder]: simmodel/
[symbol_folder]: symbol/