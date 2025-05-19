# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file . Save each script in a file with a .bat extension. Ensure you have the necessary permissions to perform the operations. Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "my-folder"

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/1923a03e-59af-461e-9d30-345db2b4df47)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.



## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/dbf12172-02f1-43d2-9de3-c8be622c1df0)
```
type nul > MyFile.txt
```
![image](https://github.com/user-attachments/assets/1615d178-ed46-47cc-ac89-2eeb8289438f)
List the contents of the "MyLab" directory.



## COMMAND AND OUTPUT:
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/648e9edb-9297-4c54-bee8-24a059c7d397)
Copy "MyFile.txt" to a new folder named "Backup" on the desktop.


## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/27d5bf35-e18f-4212-8025-b98d47810473)

```
copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/4bfa0401-d60b-4cf6-867b-de9b31cb54db)



## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Documents
```

```
move MyLab Documents
```
![image](https://github.com/user-attachments/assets/0b802e42-0eea-4c98-8c8f-12fb87c800e1)

## Exercise 2: Advanced Batch Scripting
Create a batch file named on the desktop. The batch file need to have a variable assigned with a desired name for ex. name="John" and display as "Hello, John".
## COMMANDS:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/6a267266-f87b-4c02-8af4-9c721b56430e)


## COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```


## OUTPUT
![image](https://github.com/user-attachments/assets/303d12c3-09e9-40bc-b95b-34e532f10d3d)




## RESULT:
The commands/batch files are executed successfully.

