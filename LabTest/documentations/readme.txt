Important:
To make sure data logging function correctly with shared variable(s),
you need to set a specific custom address for "My Computer" in LabVIEW Project Explorer,
Right click "My Computer" >> Properties >> Under "General" tab >> Tick "Specific custom address" >> Set the address to the same address as your myRIO device

In LabVIEW Project Explorer, you should have:
Under "My Computer":	A library that contain your variable(s) for data logging purpose [DataLogLib.lvlib]
			A .vi file for data logging [DataLog.vi]
			A text file for your data logging [DataLog.txt]
Under "myRIO" :	A Main.vi to run the myRIO device and carry out necessary operation(s).

Notes:
The function "Wait (ms)" should only be connected to integer data type, connecting it to a double (DBL) data type would results in an implicit casting.
Before your first time running the .vi file for data logging [DataLog.vi], you need to set the directory for your text file for data logging [DataLog.txt].
File name inside the square brackets [] serves only as an example, you can rename the file to anything you like. 