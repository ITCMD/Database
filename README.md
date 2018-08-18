# Database
Allows you to create and manage databases in Batch Code

# The Help File
```This is a help file created by IT Command.
To view this help file (in color) in the program use /Help
We recommend reading this in full screen mode.


Creating a Database:
  create [DBName] [Values]

 [DBName]         - Replace with the name of your database. Should be one word and have only letters and numbers.
 [Values]         - Replace with Values you wish your Database to have (up to nine values).

Example:  create People username password
    This will create a database called people with the values username and password.


Storing data in a Database:
 store [DBName] ["Value=Data"] ["Value=Data"]

 [DBName]         - Replace with the name of your existing database.
 ["Value=Data"]   - Replace Value with the preset value. Replace Data with the data you wish to assign to the value.
                    NOTE: Always keep in quotes

Example:  store People "username=Lucas" "password=1234"
    This will add a new entry into the database People with the the username Lucas and password 1234


Reading a Database
 read  [DBName] where ["value=data"] [value]

 [DBName]         - Name of the database. With just this command it will display all info in the database
  where           - The where option allows you to find a value where another value is true
 ["value=data"]   - Just like storing data, you enter the value name and the data, except it will check for sections where this is true
                   NOTE: If there are multiple instances it will select the second option. This will be changed in a future update.
 [value]          - Replace with the value you wish to get from the collumn where the value is equal to your data.
                   NOTE: You can also enter #value as the value, and it will return the #value number, which is an incrementing number given to each entry.

Example:  read People where "username=Lucas" password
    This will search for a column in the People database with the username Lucas, and will return with the password.


Removing Data from a Database
  remove [DBName] [where/#Value] ["value=data"]/[#value]

 [DBName]         - Name of the database.
  where           - Sets to where mode, which you can use like where in the READ command.
  #value          - Sets to value mode, where you enter in the #value
 ["value=data"]   - Just like storing data, you enter the name and the data, except this will remove all collumns with this true. For use with where mode only.
 [#value]         - Replace witht he value number for the entry you wish to remove. For use with Value mode only.


Deleting a Database
 delete  [DBName]

 [DBName]         -Name of the database to delete.


Errorlevels

1- Database was not found (or was found if creating a database)
2- Invalid Syntax
3- Connection Error
4- Field not found in Database (value not found)
5- No Results (not necessarely and error)



TroubleShooting
Try these commands when troubleshooting:

 update
  -Downloads the latest version of this program.

 cleanup
  -Cleans up temporary files. May remove bugs.

 clearall
  -Deletes all Databases. For use in a batch file use " Clearall Force" to bypass prompt.


This Version: 
Written by: Lucas Elliott with IT Command www.itcommand.tech
Contact:  Lucas@ITCommand.tech```

