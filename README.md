# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.


## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
```
mkdir %userprofile%\Desktop\MyLab
```
![os 1](https://github.com/hemreddy2005/Windows-basic-commands-batchscript/assets/145633111/35388694-4606-485b-aca8-7849ef2b85fb)

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![os 2](https://github.com/hemreddy2005/Windows-basic-commands-batchscript/assets/145633111/403ca7e2-1f8a-4e9f-90d8-49922a9dd02d)
![os 3](https://github.com/hemreddy2005/Windows-basic-commands-batchscript/assets/145633111/177cd8b1-12e7-4da9-8b3e-a723da8b11e8)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![os 4](https://github.com/hemreddy2005/Windows-basic-commands-batchscript/assets/145633111/46827070-bb8e-4634-83cd-2df4302bc882)

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![os 5](https://github.com/hemreddy2005/Windows-basic-commands-batchscript/assets/145633111/4549db1f-7cdb-453f-9b48-49b51e781679)
![os 6](https://github.com/hemreddy2005/Windows-basic-commands-batchscript/assets/145633111/0e0a9956-d0c9-46ba-9fa7-ef43080a0697)

## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![os 7](https://github.com/hemreddy2005/Windows-basic-commands-batchscript/assets/145633111/7419ffc4-3f49-4738-91b7-f32ecaa48433)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

## OUTPUT

![os 8](https://github.com/hemreddy2005/Windows-basic-commands-batchscript/assets/145633111/983c3d33-e17d-413d-ae1e-57583aa33a2e)

# RESULT:
The commands/batch files are executed successfully.

