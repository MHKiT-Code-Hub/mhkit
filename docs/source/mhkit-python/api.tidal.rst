.. _tidal_api:

Tidal Module
^^^^^^^^^^^^^^^^^^^^^^^^^^
The tidal module contains a set of functions to 
calculate quantities of interest for tidal energy converters (TEC).

The tidal module uses timeseries data of velocity and direction.


* **Velocity/ direction time series data** is stored as a pandas DataFrame indexed by time.
    Time can be specified in datetime or in seconds.  The column names describe the type of data in each column.

.. This doesn't generate anything
.. automodule:: mhkit.tidal
    :members:
    :no-undoc-members:
    :show-inheritance:
    
IO
""""""""""""
The io submodule contains the following functions to
load NOAA velocity/ direction data

.. autosummary::
   :nosignatures:
      
   ~mhkit.tidal.io.noaa.request_noaa_data
   ~mhkit.tidal.io.noaa.read_noaa_json


.. automodule:: mhkit.tidal.io
    :members:
    :undoc-members:
    :show-inheritance:
    
Resource
""""""""""""
The resource module allows the user to calculate the ebb and flood directions
of the tidal resource given a timeseries of directional data. 

.. autosummary::
   :nosignatures:

   ~mhkit.tidal.resource.principal_flow_directions
   ~mhkit.tidal.resource.Froude_number
   ~mhkit.tidal.resource.exceedance_probability
   
.. automodule:: mhkit.tidal.resource
    :members:
    :undoc-members:
    :show-inheritance:

.. autofunction:: mhkit.tidal.resource.Froude_number    
.. autofunction:: mhkit.tidal.resource.exceedance_probability

Performance
""""""""""""
The performance submodule contains functions to compute equivalent diameter
and capture area for circular, ducted, rectangular, adn multiple circular devices.
A circular device is a vertical axis water turbine (VAWT). A
rectangular device is a horizontal axis water turbine (HAWT). A ducted device
is an enclosed VAWT. A multiple-circular devices is a device with
multiple VAWTs per device. This submodule also contains functions for computing 
the tip speed ratio and power coefficient from a blade/rotor type device.


.. autosummary::
   :nosignatures:

   ~mhkit.tidal.performance.circular
   ~mhkit.tidal.performance.ducted
   ~mhkit.tidal.performance.rectangular
   ~mhkit.tidal.performance.multiple_circular
   ~mhkit.tidal.performance.tip_speed_ratio
   ~mhkit.tidal.performance.power_coefficient
   ~mhkit.tidal.performance.power_curve
   ~mhkit.tidal.performance.device_efficiency
   ~mhkit.tidal.performance.velocity_profiles
   
   
.. automodule:: mhkit.tidal.performance
    :members:
    :undoc-members:
    :show-inheritance:

.. autofunction:: mhkit.tidal.performance.circular
.. autofunction:: mhkit.tidal.performance.ducted
.. autofunction:: mhkit.tidal.performance.rectangular
.. autofunction:: mhkit.tidal.performance.multiple_circular
.. autofunction:: mhkit.tidal.performance.tip_speed_ratio
.. autofunction:: mhkit.tidal.performance.power_coefficient

	
Graphics
""""""""""""
The graphics submodule contains functions to plot tidal resource data 
and related metrics.

.. autosummary::
   :nosignatures:

   ~mhkit.tidal.graphics.plot_rose
   ~mhkit.tidal.graphics.plot_joint_probability_distribution
   ~mhkit.tidal.graphics.plot_current_timeseries
   ~mhkit.tidal.graphics.plot_velocity_duration_curve
   ~mhkit.tidal.graphics.tidal_phase_probability
   ~mhkit.tidal.graphics.tidal_phase_exceedance
   
.. automodule:: mhkit.tidal.graphics
    :members:
    :undoc-members:
    :show-inheritance:
    
.. autofunction:: mhkit.tidal.graphics.plot_velocity_duration_curve    
   :noindex:



