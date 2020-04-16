			SMART DEREGISTRATION PREDICTION
Functions used:-

app2.mlapp - Main file of MATLAB's app builder readable type. Contains code related various graphical interfaces such 
		as  sliders, buttons, inputs boxes. Objective of few of these functions are listed below-

	startupFcn(app) - plots the membership function graph based on the default values.

	GETRESULTButtonPushed(app,event)- Takes the current configuration of membership functions, weights and input 
					parameters and apply fuzzy logic operation and predefined ruleset to get 
					deregistration status.

	importButtonPushed(app,event)- Open file explorer to allow users to browse through computer to input required 
					.csv files ( format- column 1,2 and 3 having noramlised values of attendance, 
					marks and current cgpa respectively), then it creates a RESULT.csv in the 
					same directory which contains deregistration details for every entry. 
 
	XYZ_ValueChanged(app,event)- Contains code for corresponding XYZ slider which changes the respective plot of 
					membership function upon change in position of slider.

val.m - Supporting file containing function which calls other supporting functions, namely zero_part, 
	low_part and high_part , depending upon the current rule.

zero_part - Supporting file containing function which generates membership value if the lingustic variable corresponds 
		to "low." 


low_part - Supporting file containing function which generates membership value if the lingustic variable corresponds 
		to "avg." 


high_part - Supporting file containing function which generates membership value if the lingustic variable corresponds 
		to "high." 

----------------------------------------------------------------------------------------------------------------------


			SMART GRADE PREDCITION
File name - gui.py


Functions used for the implementation of the model training:-

tra() - function used for training the model. The function takes the input file, performs smote transformation on the data and then performs one hot encoding on the output values.
After splitting the input into train and test data, the 4*8*4 neural network model is trained and tested. 


Functions used for creating the GUI interface:-

load_csv() - Loads the csv into memory
write_csv() - Saves the csv into the system
remove_Row() - removes a row from csv
add_Row() - adds a row into csv
remove_Column() - removes a row from csv
add_Column() - adds a row into csv
contextMenuEvent() -  handles the menu options
handle_request() - handles a particular request


My_window - Class implementing all the operations
main - Object of the class

