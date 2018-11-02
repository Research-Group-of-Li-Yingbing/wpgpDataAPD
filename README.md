# wpArcToolbox
ESRI Add-in that allows users to download rasters from WorldPop FTP server.

Package: wpArcToolbox
Type: ArcGIS Addin / Python Toolbox
Vesion: 0.1
Author: David Kerr <David.Kerr@soton.ac.uk> Maksym Bondarenko <M.Bondarenko@soton.ac.uk> Nik Ves <N.Ves@soton.ac.uk> and Alessandro Sorichetta <A.Sorichetta@soton.ac.uk>
Maintainer: David Kerr <David.Kerr@soton.ac.uk>
Depends: ArcMap 10.1 or greater
Description: ArcMap AddIn button and Python toolbox enabling users to download raster from WorldPop FTP and add them to ArcMap session.
License: The WorldPop datasets are licensed under the Creative Commons Attribution 4.0 International License.


## Installation
- The Add-in and associated Python Toolbox can be installed by downloading and double-clicking the 'WPDwnld_btn.esriaddin' file. No other files are needed for installation. This will install the add-in into the Add-ins folder:

```
 C:\Users\<username>\Documents\ArcGIS\AddIns\Desktop10.1
```

- Users who want to make use of the Python Toolbox should download the Install folder. Using ArcMap's Catalog, navigate to the WPdownload.pyt file inside this folder to access the Toolbox and associated download tool.

- This tool requires an internet connection to work, and will raise an error before launching if no connection is found.

##Instructions

### Addin
- Following installation, open new session of ArcMap, or open Map document in which to download rasters. 
- If Addin button does not show on interface, click Customize > Toolbars > WP Covariate Download Toolbar.
- Click WP button to open download wizard
- If Python window is open, the following error may be displayed:

```
TypeError: GPToolDialog() takes at most 1 argument (2 given)
```

This can be ignored. See Issues below.
- Select country
- Select layer to download
- Select path to folder in which to download raster
- Check box if raster should be added to the current map document following download
- Click 'Okay' to start download.


## Issues
When clicking the Add-in button on the interface, the following error is produced in the ArcMap Python terminal:

```
TypeError: GPToolDialog() takes at most 1 argument (2 given)
```

This is a bug known to ESRI and is logged under issue no. NIM089253. This error can be ignored.





