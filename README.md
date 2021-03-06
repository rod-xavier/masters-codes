# masters-codes
In this repository one can find the codes used during my Master's programs of the Federal University of São Paulo.

The research consists of irradiance forecast using satellite imagery on a timeframe of around 3 hours, focusing on 4 different locations in the brazilian territory.
The forecasted images are obtained with the use of the Optical Flow tool, available in the cv2 python library.
Feel free to use anything, improvement sugestions are highly appreciated.

As of the present moment, the codes can be summarized as it follows:

exploratory_analysis: this code uses data collected by surface weather stations, deals with outliers and plots information regarding meteorological variables such as temperature, precipitation and global radiation annual cycles in 4 different locations.

optical_flow: this code uses as input NetCDF files of Goes-16 satellite imagery (visible channel), and the outputs are forecasted images with optical flow and the goodness of fit os said forecasts, using the Constanza (1989) method.

clear_sky: this code uses as input NetCDF files of Goes-16 satellite imagery, a certain year and a list of months and locations of interest. The output consists of composite clear sky images, with the purpose of producing a clear sky day cycle of the desired locations.

irradiance_forecast_optical_flow: this is the final algorithm, still under construction, it takes a location (latitute, longitude, altitude) and a .nc extension file, calculates the optical flow and finally, display a 2 hour forecast of global horizontal irradiance, comparing it with real observed data and the persistence method.
