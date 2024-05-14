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
![Screenshot 2024-04-28 111358](https://github.com/Bakkiyalakshmiethiraj/Windows-basic-commands-batchscript/assets/144870983/e41be42e-04ae-4c0e-a73a-26f6e0cb24de)

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![Screenshot 2024-04-28 111523](https://github.com/Bakkiyalakshmiethiraj/Windows-basic-commands-batchscript/assets/144870983/0650cf9c-e47d-4b60-89f1-141e73e567a5)
![Screenshot 2024-04-28 111602](https://github.com/Bakkiyalakshmiethiraj/Windows-basic-commands-batchscript/assets/144870983/bda931d8-f9ca-416e-98a4-e1f3d937e58a)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![Screenshot 2024-04-28 111717](https://github.com/Bakkiyalakshmiethiraj/Windows-basic-commands-batchscript/assets/144870983/43d07dad-f573-46ee-811a-06f2eb6dd350)

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![Screenshot 2024-04-28 111858](https://github.com/Bakkiyalakshmiethiraj/Windows-basic-commands-batchscript/assets/144870983/cc16de8d-c901-4806-a527-a5548c58f0cc)

## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![Screenshot 2024-04-28 112034](https://github.com/Bakkiyalakshmiethiraj/Windows-basic-commands-batchscript/assets/144870983/d0c431ee-68e2-4633-8da0-3c4aa484df1e)


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

![Screenshot 2024-04-28 125525](https://github.com/Bakkiyalakshmiethiraj/Windows-basic-commands-batchscript/assets/144870983/3c54adaa-b5af-4db8-973f-c7d616cd9e91)




# RESULT:
The commands/batch files are executed successfully.

