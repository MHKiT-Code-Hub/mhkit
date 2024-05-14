.. _release_notes:

Release Notes
=============

MHKiT-Python v0.8.0
-------------------
MHKiT-Python v0.8.0 adds the following modules and capabilities to MHKiT-Python:

 * Support for python 3.10 and 3.11
 * Support for xarray input and output across all MHKiT functions
 * Wave module enhancements:
    - Automatic Threshold Calculation for Peaks-Over-Threshold
    - Wave Heights Analysis
    - Enhanced Zero Crossing Analysis
 * DOLfYN enhancements:
    - Altimeter Support
    - Data Handling Improvements
    - Instrument Noise Subtraction
    - Improved File Handling
 * River and Tidal - D3D:
    - Added limits to variable_interpolation and added 3 array input capability to create_points
 * Developer Experience:
    - Black formatting
    - Linting and type hints
    - CI/CD improvements
 * General upkeep and compatibility maintenance
 * General Bug Fixes


MHKiT-Python v0.7.0
-------------------
MHKiT-Python v0.7.0 adds the following modules and capabilities to MHKiT-Python:

 * Mooring Module: We are pleased to introduce the new mooring module. This addition primarily supports outputs from MoorDyn. Within this module, users can:
    - Import data
    - Calculate lay length
    - Visualize mooring line movements in 2D and 3D with graphical animations.
    - Accompanying this module is an example notebook to guide users on its functionalities.
 * Dolfyn Module Revamp: The Dolfyn module has been overhauled. Enhancements include:
    - Turbulence calculation capability
    - Performance measures for tidal power as outlined in IEC/TS 6200-200.
 * New Contributions: A big shoutout to our community member, @mbruggs, for adding the ability to compute surface elevation using IFFT.
 * NDBC Buoy Metadata: Users can now fetch NDBC buoy metadata directly through MHKiT.
 * Delft3D Module Update: Stay up to date with support for the latest Delft3D NetCDF format.
 * Provide a function to convert from Te to Tp using ITTC approximation
 * General upkeep and compatibility maintenance
 * General Bug Fixes


MHKiT-Python v0.6.0
-------------------
MHKiT-Python v0.6.0 adds the following modules and capabilities to MHKiT-Python:

 * Test Suite Restructure: improved the ability to run and edit tests by breaking them out from single files into folders containing tests for specific parts of each submodule
 * Added a metocean module which can pull data from the wind_toolkit with 4 regions and 1-hr or 5-min data
 * Two DOLfYN updates address bug fixes, clean up, and some feature expansion:
    - ADV skipped timesteps, max gap, and attributes
    - error in integral length scale calculation
    - error in despiking function
    - move Reynolds stress and cross-spectral density calculations to ADV folder
    - prevent inaccurate TKE calculation from ADCP velocity input
 * Delft3D z-calculation, timestep, and new example notebook comparing ADV, and D3D river transect data
 * WEC-Sim v5.0 support
 * Return period added for contours
 * Provide a function to convert from Te to Tp using ITTC approximation
 * General upkeep and compatibility maintenance
 * General Bug Fixes


MHKiT-Python v0.5.0 & MHKiT-Matlab v0.4.0
-----------------------------------------
MHKiT-Python v0.5.0 adds the following modules and capabilities to MHKiT-Python:

 * Organization: grouped io specific functions in wave, tidal, and river into io folder
 * Updated Jonswap spectrum to match IEC guidance
 * `dolfyn <https://mhkit-software.github.io/MHKiT/mhkit-python/api.dolfyn.html#dolfyn>`_ Added DOLfYN module to analyze and process ADV and ADCP data
 * `wave.contours <https://mhkit-software.github.io/MHKiT/mhkit-python/api.wave.html#contours>`_ Incorporated the remaining WDRT functionality
 * `river.io.d3d <https://mhkit-software.github.io/MHKiT/mhkit-python/api.river.html#io>`_ Added Delft3D case post-processing in the river/ tidal models
 * Fixed a bug in the wave elevation function 
 * Include the last day in CDIP requests and file timezone issues with CDIP
 * Upgrades to processing numpy and pandas version to maintain compatability

MHKiT-Matlab v0.4.0 adds the following modules and capabilities to MHKiT-MATLAB:

 * Updated Jonswap spectrum to match IEC guidance
 * `cdip <https://mhkit-software.github.io/MHKiT/mhkit-matlab/api.wave.html#io>`_ Module: functions for downloading and converting CDiP data into MHKIT formats.
 * `WPTO hindcast <https://mhkit-software.github.io/MHKiT/mhkit-matlab/api.wave.html#io>`_ Module: functions for downloading and converting WPTO Hindcast data into MHKIT formats
 * Fixed a bug in the wave elevation function 


MHKiT v0.4.0
-------------
MHKiT v0.4.0 adds the following modules and capabilities to MHKiT:

 * `wave.io.cdip <https://mhkit-software.github.io/MHKiT/mhkit-python/api.wave.html#io>`_ Module: functions for downloading and converting CDiP data into MHKIT formats (MHKiT-Python Only).
 * `wave.io.hindcast <https://mhkit-software.github.io/MHKiT/mhkit-python/api.wave.html#io>`_ Module: functions for downloading and converting WPTO Hindcast data into MHKIT formats (MHKiT-Python Only).
 * `wave.io.swan <https://mhkit-software.github.io/MHKiT/mhkit-python/api.wave.html#io>`_ Module: functions for importing and converting SWAN data into MHKIT formats.
 * `wave.resource <https://mhkit-software.github.io/MHKiT/mhkit-python/api.wave.html#resource>`_ Module: Deep water approximations for wave resource characterization (MHKiT-Python Only).
 * `utils <https://mhkit-software.github.io/MHKiT/utils.html#Utils>`_ Module: Vector averaging capabilities in statistics calculations. 
 * `wave.performance <https://mhkit-software.github.io/MHKiT/mhkit-python/api.wave.html#performance>`_ Module: Wave power performance workflow functions.


MHKiT v0.3.1
-------------
 * Ensures compatibility with dependency PECOS v0.1.9 


MHKiT v0.3.0
-------------
MHKiT v0.3.0 adds the following modules to MHKiT:

 * `wave.io.ndbc <https://mhkit-software.github.io/MHKiT/mhkit-python/api.wave.html#io>`_ Module: functions for downloading and converting NDBC data into MHKIT formats.
 * `wave.io.wecsim <https://mhkit-software.github.io/MHKiT/mhkit-python/api.wave.html#io>`_ Module: functions for converting WEC-Sim data into MHKiT formats.
 * `river.performance <https://mhkit-software.github.io/MHKiT/mhkit-python/api.river.html#performance>`_ and `tidal.performance <https://mhkit-software.github.io/MHKiT/mhkit-python/api.tidal.html#performance>`_ Module: new functionality to assess device performance from blade/rotor type devices.
 * `Loads Module <https://mhkit-software.github.io/MHKiT/mhkit-python/api.loads.html#loads-module>`_: new function for computing blade moments; new submodule structure `loads.general <https://mhkit-software.github.io/MHKiT/mhkit-python/api.loads.html#general>`_ and `loads.graphics <https://mhkit-software.github.io/MHKiT/mhkit-python/api.loads.html#graphics>`_.

Refer to the following GitHub repositories to access the MHKiT v0.3.0 tagged release:

MHKiT-Python v0.3.0 
^^^^^^^^^^^^^^^^^^^^^
* `MHKiT-Python v0.3.0 Release <https://github.com/MHKiT-Software/MHKiT-Python/releases/tag/v0.3.0>`_
* .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4063895.svg
     :target: https://doi.org/10.5281/zenodo.4063895

MHKiT-MATLAB v0.3.0 
^^^^^^^^^^^^^^^^^^^^^
* `MHKiT-MATLAB v0.3.0 Release <https://github.com/MHKiT-Software/MHKiT-MATLAB/releases/tag/v0.3.0>`_
* .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4063920.svg
     :target: https://doi.org/10.5281/zenodo.4063920

MHKiT v0.2.0
-------------
MHKiT v0.2.0 adds the following modules to MHKiT:

* :ref:`power`: Calculate quantities of interest for power production and power quality
* :ref:`loads`: Calculate quantities of interest for mechanical loads assessments

This release also includes minor updates to the wave module to improve the versatility of the module. Refer to the following GitHub repositories to access the MHKiT v0.2.0 tagged release:

MHKiT-Python v0.2.0 
^^^^^^^^^^^^^^^^^^^^^
* `MHKiT-Python v0.2.0 Release <https://github.com/MHKiT-Software/MHKiT-Python/releases/tag/v0.2.0>`_  
* .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3924684.svg
     :target: https://doi.org/10.5281/zenodo.3924684

MHKiT-MATLAB v0.2.0 
^^^^^^^^^^^^^^^^^^^^^
* `MHKiT-MATLAB v0.2.0 Release <https://github.com/MHKiT-Software/MHKiT-MATLAB/releases/tag/v0.2.0>`_ 
* .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3928406.svg
     :target: https://doi.org/10.5281/zenodo.3928406


MHKiT v0.1.0
-------------
The first official release of MHKiT, developed in Python and MATLAB, includes the following modules:

* :ref:`qc`: Perform quality control analysis
* :ref:`wave`: Calculate quantities of interest for wave energy converters (WEC)
* :ref:`river`: Calculate quantities of interest for river energy converters (REC)
* :ref:`tidal`: Calculate quantities of interest for tidal energy converters (TEC)
* :ref:`utils`: Includes helper functions

The v0.1.0 release includes methods for resource assessment, device performance, graphics, io and quality control. Refer to the following GitHub repositories to access the MHKiT v0.1.0 tagged release:

MHKiT-Python v0.1.0 
^^^^^^^^^^^^^^^^^^^^^
* `MHKiT-Python v0.1.0 Release <https://github.com/MHKiT-Software/MHKiT-Python/releases/tag/v0.1.0>`_

MHKiT-MATLAB v0.1.0 
^^^^^^^^^^^^^^^^^^^^^
* `MHKiT-MATLAB v0.1.0 Release <https://github.com/MHKiT-Software/MHKiT-MATLAB/releases/tag/v0.1.0>`_
