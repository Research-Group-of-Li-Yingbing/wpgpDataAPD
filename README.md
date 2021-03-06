[![N|Solid](http://maps.worldpop.org.uk/img/worldpop-logo.png)](http://www.worldpop.org.uk/)

# wpgpDataAPD


## Introduction

wpgpDataAPD is an ESRI plugin/ArcPy Python toolbox that allows users to download rasters from [WorldPop](http://www.worldpop.org.uk/) FTP server using ArcMap.

The [WorldPop](http://www.worldpop.org.uk/) Global High Resolution Population Denominators Project, funded by the Bill and Melinda Gates Foundation (OPP1134076), has produced an open-access archive of 3-arc seconds (approximately 100m at the equator) gridded population datasets, also structured by gender and age groups, for 249 countries, dependencies, and territories for 21-years (2000-2020), using the methods described by Stevens et al., 2015 (<https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0107042>), Gaughan et al., 2016 (<https://www.nature.com/articles/sdata20165>), and Pezzulo et al., 2017 (<https://www.nature.com/articles/sdata201789>). In addition, the project has also made available the covariate datasets used as inputs to produce the gridded population datasets (Lloyd et al., under review). These datasets are available for download from the [WorldPop](http://www.worldpop.org.uk/) website and FTP server using a range of methods and tools.


- **Package**: wpgpDataAPD
- **Type**: ArcGIS Addin / Python Toolbox
- **Vesion**: 0.1
- **Developed by**: [WorldPop](http://www.worldpop.org.uk/) SDI Team (David Kerr [*Main developer*], Maksym Bondarenko, Nik Ves and Alessandro Sorichetta)
- **Maintainer**: David Kerr 
- **Depends**: ArcMap 10.1 or higher (ArcGIS Pro currently not supported)
- **Description**: ArcMap AddIn button and Python toolbox enabling users to download rasters from [WorldPop](http://www.worldpop.org.uk/) FTP and add them to an ArcMap session.
- **License**: The [WorldPop](http://www.worldpop.org.uk/) datasets are licensed under the Creative Commons Attribution 4.0 International License.


## Installation
- The Add-in and associated Python Toolbox can be installed by downloading and double-clicking the 'WPDwnld_btn.esriaddin' file. No other files are needed for installation. This will install the add-in into the Add-ins folder:

```
 C:\Users\<username>\Documents\ArcGIS\AddIns\Desktop10.1
```

- Users who want to make use of the Python Toolbox should download the Install folder (the 'WPDwnld_btn.esriaddin' file is not needed in these instances). Using ArcMap's Catalog, navigate to the WPdownload.pyt file inside this folder to access the Toolbox and associated download tool.

- This tool requires an internet connection to work, and will raise an error before launching if no connection is found.

## Instructions

- Following installation, open new session of ArcMap, or open Map document in which to download rasters. 
- If Addin button does not show on interface, click Customize > Toolbars > WP Covariate Download Toolbar.
- Click WorldPop iconised button to open download wizard
- If Python window is open, the following error may be displayed:

```
TypeError: GPToolDialog() takes at most 1 argument (2 given)
```

This can be ignored. See Issues below.
- Select country/territory
- Select layer to download
- Select path to folder in which to download raster
- Check box if raster should be added to the current map document following download
- Click 'Okay' to start download.


## Issues
When clicking the Add-in button on the interface, the following error is produced in the ArcMap Python terminal:

```
TypeError: GPToolDialog() takes at most 1 argument (2 given)
```

This is a bug known to ESRI and is logged under issue no. [NIM089253](https://support.esri.com/en/bugs/nimbus/TklNMDg5MjUz). This error can be ignored.





