# Farm Management System

A comprehensive Java-based desktop application for managing farm operations, including employee management, activity tracking, expense management, and profitability analysis.

## Features

- **User Authentication**: Secure login system with user role management
- **Employee Management**: Add, update, and track employee information
- **Activity Tracking**: Monitor farm activities and operations
- **Expense Management**: Track and categorize farm expenses
- **Deduction Management**: Manage employee deductions and allowances
- **Salary Management**: Calculate and manage employee salaries
- **Location Management**: Manage multiple farm locations
- **Profit Analysis**: Analyze and view gross profit metrics
- **Database Management**: Robust MySQL database integration
- **User Management**: Manage user accounts and permissions

## Technology Stack

- **Language**: Java
- **GUI Framework**: Swing
- **Database**: MySQL
- **Build Tool**: Ant
- **IDE**: NetBeans

## Project Structure

```
src/farmmanagementsystem/
├── FarmManagementSystem.java       # Main entry point
├── SplashScreen.java               # Splash screen UI
├── db/                             # Database connectivity
│   ├── DBConnection.java
│   ├── DBQuery.java
│   └── JFrameLogin.java
├── gui/                            # GUI components
│   ├── MainMenu.java
│   ├── Login.java
│   ├── ManageEmployee.java
│   ├── ManageActivity.java
│   ├── ManageExpense.java
│   ├── ManageLocation.java
│   ├── ManageSalary.java
│   ├── ManageDeduction.java
│   ├── ManageGrossProfit.java
│   ├── ManageUser.java
│   └── ChangePassword.java
├── model/                          # Data models
│   ├── Employee.java
│   ├── Activity.java
│   ├── Expenses.java
│   ├── Location.java
│   ├── Salary.java
│   ├── Deduction.java
│   ├── GrossProfit.java
│   ├── User.java
│   ├── Claim.java
│   └── Log.java
└── util/                           # Utility classes
    ├── Database_Configuration.java
    ├── DateConverter.java
    ├── FileEditor.java
    └── ComponentHouseResizer.java
```

## Prerequisites

- Java Development Kit (JDK) 8 or higher
- MySQL Server 5.7 or higher
- Apache Ant (for building)

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/NalamothuLokesh/FarmEasy.git
   cd FarmEasy
   ```

2. **Set up the database**
   - Create a MySQL database using the provided SQL file
   - Import the database schema:
     ```bash
     mysql -u root -p < "New Project 20211224 1100.sql"
     ```

3. **Configure database connection**
   - Open `src/farmmanagementsystem/util/Database_Configuration.java`
   - Update the database credentials (hostname, username, password, database name)

4. **Build the project**
   ```bash
   ant build
   ```

5. **Run the application**
   ```bash
   ant run
   ```

## Usage

1. Launch the application
2. Login with your credentials (default admin user credentials may apply)
3. Navigate through the menu options to:
   - Manage employees
   - Track activities
   - Record expenses
   - View profit metrics
   - Manage user accounts

## File Descriptions

- **build.xml**: Ant build configuration
- **manifest.mf**: JAR manifest file
- **New Project 20211224 1100.sql**: Database schema and initial data

## Building a JAR File

To create a distributable JAR file:
```bash
ant jar
```

The compiled JAR will be in the `dist/` directory.

## License

This project is provided as-is for farm management purposes.

## Author

Lokesh - NalamothuLokesh

## Support

For issues or questions, please create an issue on the GitHub repository.
