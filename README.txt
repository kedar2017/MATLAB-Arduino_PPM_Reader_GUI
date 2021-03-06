Instructions:
By Gabriel Staples
README last updated: 4 May 2014

For a demo of this code live in action, go here: http://www.instructables.com/id/Arduino-to-MATLAB-GUI-Live-Data-Acquisition-Plotti/

1) Upload the Arduino code to your Arduino.  
-open the "MATLAB_to_Arduino1_0.ino" code to do so
2) Connect your RC Tx's trainer port to your Arduino, as follows:
	a) Connect trainer ground to Arduino GND.  Refer to this list for pinout help: http://www.mftech.de/buchsen_en.htm
	b) Connect the trainer PPM out to the Arduino D2 pin, with a 1KOhm resistor in series, for protection in case you make a mistake while probing stuff.
3) Run the MATLAB code, by running the file called "MATLAB_to_Arduino_GUI_driver.m".
-Note: to edit the GUI, use MATLAB's GUI editor called "guide."  Open guide by typing "guide" in the MATLAB workspace, then open the "MATLAB_to_Arduino_GUI_driver.fig" file via guide.
	a) Once you have run "MATLAB_to_Arduino_GUI_driver.m," the GUI will pop up.  Type in the appropriate COM port address to your Arduino, and press the "Start" button.  
	b) Data will automatically begin to show up, so long as your Tx is on.  Move the sticks to see the output.  To look at your logged data file, go to the "MATLAB GUI PPM Reader 1.0\data" folder.  The data file names will look something like this: "data_20140504_0003_05".  The numbers are the time stamp of when the file was made, in order of [year, month, day]_[hour, minute]_second.csv.  
	c) The data file (ending in .csv) is a comma-delimited standard ASCII text file.  Since it ends in the .csv file extension, if you simply double click it, it will automatically open up in Microsoft Excel, where you can easily plot and manipulate the data.
	
