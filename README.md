# using-csv-files
Exercise 3 of the "Intermediate Object-Oriented Programming for Unity Games" course of the "C# Programming for Unity Game Development" Specialization by the University of Colorado via Coursera

## Description

Problem 1 – Start using the ConfigurationDataConfigurationData class

Add a static field to the ConfigurationUtilsConfigurationUtils class to hold a ConfigurationDataConfigurationData object.

Add code to the ConfigurationUtilsConfigurationUtils InitializeInitialize method to call the ConfigurationDataConfigurationData constructor to populate your new field. Change all the ConfigurationUtilsConfigurationUtils properties to return the appropriate properties from your new field instead of the hard-coded values they currently return.

Run your game. It should work just like it did before you made these changes.

Problem 2 – Create the configuration data file

Create a new StreamingAssets folder (capitalize it exactly as shown) in your Project window; this is where you’ll save your csv file. Putting the file there makes it automatically get included in our build and also makes it so we can use Application ⁣ ⁣. ⁣ ⁣streamingAssetsPathApplication.streamingAssetsPath to get the file location from our script, which will work both in the editor and if you distribute your game.

Create a csv (comma-separated value) file containing the configuration data; you should call it ConfigurationData.csv (or you can change the file name in the ConfigurationDataConfigurationData class). The first line in the file should be a comma-separated list of the value names and the second line in the file should be a comma-separated list of the values. This is the format you’d expect to see exported from a spreadsheet that game designers were using to tune the game. The ConfigurationDataConfigurationData class only has two fields for configuration data, so you only need to include names and values for those two fields in the file. 

Save the csv file in your StreamingAssets folder.

Problem 3 – Use configuration data from file

Add code to the ConfigurationDataConfigurationData constructor to open the configuration data file using Application ⁣ ⁣. ⁣ ⁣streamingAssetsPathApplication.streamingAssetsPath and your file name as the full file name. Be sure to include this code in an exception handler. You should have a catch block that catches all exceptions (but doesn’t do anything in the catch block) and you should have a finally block that closes the file if it’s not null. You’ll need to add a System ⁣ ⁣. ⁣ ⁣IOSystem.IO using directive to get access to the StreamReaderStreamReader class and a SystemSystem using directive to get access to the ExceptionException class.

Add code to extract the values from the second line in the file and populate the fields with them. You should do this in the SetConfigurationDataFieldsSetConfigurationDataFields method I provided in the ConfigurationDataConfigurationData class.

When you run your, game it should work just like it did before this step.

## Getting Started

n/a

### Dependencies

* Windows 10
* Microsoft Visual Studio
* .NET
* Unity

### Installing

* Download link: [Github Repository](https://github.com/lyndonpanton/using-csv-files)

### Executing program

n/a

## Help

n/a

## Authors

Lyndon Mykal Panton
[lyndonpanton](https://github.com/lyndonpanton/)

## Version History

* 0.1
    * Initial Release

## License

n/a

## Acknowledgments

Problem provided by the _University of Colorado_ and _Coursera_
