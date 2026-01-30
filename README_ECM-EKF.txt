- The model folder contains the 4 .SLX files along with the data dictionary file "DataECM.sldd" and the "10-24-19_16.28 960_WLTP206a.mat" drivecycle file for the input for current and voltage.
- Plots folder has the result plots


How to run the models

- Open the .slx file in Simulink
- Load the 10-24-19_16.28 960_WLTP206a.mat file in command window
- Run the below code in command window
V_ts = timeseries(meas.Voltage, meas.Time);
I_ts = timeseries(meas.Current, meas.Time);
- Link the data dictionary to the model
	Go to modelling tab
	Drop down the design dialog box 
	Click on link to data dictionary
	Browse and select the data dictionary file path 
	Click ok
- Run the Simulink model