# Bash Shell Script Database Management System (DBMS)

## Project Overview
This project aims to develop a lightweight Database Management System (DBMS) using Bash scripting. The system allows users to store and retrieve data directly from the hard disk. It features a Command Line Interface (CLI) with an intuitive menu-based navigation system.

Two versions of the application are available:
- A CLI-based version.
- A GUI version implemented using Zenity.

This project was completed during our ITI internship in the Full Stack Web Development using Python 4-month intensive code camp.

## Features

### Main Menu
The main menu provides the following functionalities:
- **Create Database**: Create a new database.
- **List Databases**: Display a list of all existing databases.
- **Connect To Database**: Access a specific database for further operations.
- **Drop Database**: Delete an existing database.

### Database Menu
Upon connecting to a specific database, the following features are available:
- **Create Table**: Define a new table with user-specified columns and data types.
- **List Tables**: Display all tables in the current database.
- **Drop Table**: Delete a specific table.
- **Insert into Table**: Add new rows to a table while enforcing primary key constraints and data type validations.
- **Select From Table**: Query rows from a table and display results in a well-formatted manner.
- **Delete From Table**: Remove specific rows from a table.
- **Update Table**: Modify data in existing rows, with validations for data types.

## Implementation Details
- **Database Structure**: Databases are stored as directories in the same directory as the script file.
- **Data Validation**:
  - Column data types are defined during table creation and validated during insertion and updates.
  - Users specify a primary key during table creation, and the script enforces uniqueness for the primary key in all insert operations.
- **Select Queries**: Results are displayed in the terminal in an organized and readable format.

## Authors
- **Omar Sameh**
- **Hussein Saad**

## How to Use
1. Clone the repository:
   ```bash
   git clone git@github.com:OmarSameh2001/bash-dbms.git
   cd <repository-directory>
   ```
2. Run the CLI version:
   ```bash
   ./Gui/dbms_gui
   ```
3. Run the GUI version:
   ```bash
   ./Cli/dbms_script
   ```

## Notes
- Ensure the script has executable permissions:
  ```bash
  chmod +x ./Gui/dbms_gui ./Cli/dbms_script
  ```
- The script requires `Zenity` to be installed for the GUI version.
  ```bash
  sudo apt install zenity
  ```

## Feedback
We welcome any feedback or suggestions to improve this project. Feel free to open issues or submit pull requests.

