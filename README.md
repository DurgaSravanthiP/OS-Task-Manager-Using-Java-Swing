# 🖥️ OS Task Manager Using Java Swing
This project is a desktop-based Task Manager application built using Java Swing. It retrieves real-time running processes from the system using PowerShell commands and displays them in an interactive GUI. Users can search, refresh, and terminate processes similar to the Windows Task Manager.

## 🚀 Features
- Displays real-time process details including PID, Process Name, CPU Usage (%), and Memory Usage (MB)
- Search processes by Name or PID
- Refresh process list at any time
- Kill/terminate selected processes instantly
- Clean and simple Java Swing interface

## 🛠️ Technologies Used
- Java Swing  
- AWT  
- DefaultTableModel  
- JTable  
- PowerShell (for fetching system processes)

## 📂 Files Included
- TaskManagerTool.java → Main project source file  
- PPT - OS Task Manager using Java Swing.pdf  
- Report - OS Task Manager Using Java Swing.pdf  

## ▶️ How to Run the Project
### 1. Install Java (JDK 8 or above)
Check Java version:

java -version

### 2. Compile the program


javac TaskManagerTool.java

### 3. Run the program


java TaskManagerTool


## 📑 How It Works
### Fetching Processes
The application runs this PowerShell command internally:


Get-Process | Select-Object Name,Id,CPU,WorkingSet

### Killing a Process
When the user selects a row and clicks "Kill Process", the following command runs:


taskkill /PID <pid> /F


## 📘 Documentation Included
This repository includes a full PPT and complete project report explaining:
- System architecture  
- Java Swing UI design  
- PowerShell integration  
- Working methodology  

## 👤 Author
Durga Sravanthi  
B.Tech CSE, SRM University 
