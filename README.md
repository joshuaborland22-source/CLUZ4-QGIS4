# CLUZ4

CLUZ plugin for QGIS 4.0+

CLUZ (Conservation Land-Use Zoning software) is a QGIS plug-in that allows users to design protected area networks
and other conservation landscapes and seascapes. It can be used for on-screen planning and also acts as a link for
the Marxan conservation planning software. It was developed by Bob Smith, from the Durrell Institute of Conservation
and Ecology (DICE), and funded by the UK Government's Darwin Initiative.

More details about CLUZ are available here http://anotherbobsmith.wordpress.com/software/cluz/

## QGIS 4.0 Port

This version has been ported to QGIS 4.0 (Qt6/PyQt6) with the following changes:

- Replaced all direct `PyQt5` imports with `qgis.PyQt` compatibility layer
- Updated all Qt5-style enums to Qt6 scoped enums (e.g. `QSizePolicy.Expanding` to `QSizePolicy.Policy.Expanding`)
- Replaced `exec_()` with `exec()` throughout
- Wrapped `resources_rc` imports in try/except for robustness
- Removed deprecated `qVersion()` usage

## Installation

1. Download the latest release zip file
2. In QGIS, go to Plugins > Manage and Install Plugins > Install from ZIP
3. Select the downloaded zip file

## License

GPL v2+. See [LICENSE.md](LICENSE.md) for details.

## Original Author

Bob Smith (r.j.smith@kent.ac.uk) - Durrell Institute of Conservation and Ecology (DICE)
