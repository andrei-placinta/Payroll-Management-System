# Payroll Management System

A desktop application for employee management and payroll processing, developed using **C#, Windows Forms and Oracle Database**.

The application manages employee records, performs database-driven payroll calculations and generates salary reports.

## Features

- Employee management (add, view, update and delete records)
- Payroll processing and salary management
- Automated payroll calculations using Oracle PL/SQL triggers
- Configurable CAS, CASS and income tax rates
- Gross salary, taxable income and net salary calculations
- Bonus and deduction management
- Payroll summary reports
- Individual employee payslips
- PDF report generation

## Tech Stack

- **Programming Language:** C#
- **Desktop Framework:** Windows Forms
- **.NET Framework:** 4.5.1
- **Database:** Oracle Database
- **Data Access:** Oracle Managed Data Access (ODP.NET)
- **Database Programming:** SQL, PL/SQL
- **Reporting:** Crystal Reports

## Database Logic

Oracle PL/SQL triggers handle payroll calculations when employee records are inserted or updated.

The calculation process includes:

- Gross salary based on base salary, salary supplements and bonuses.
- CAS and CASS contributions.
- Taxable gross income.
- Income tax calculation.
- Net salary after contributions, taxes and additional deductions.

Contribution and income tax rates are stored in the database and can be configured through the application.

## Project Structure

```text
payroll-app-main/
│
├── WindowsFormsApplication10/
│   ├── Program.cs
│   ├── Form1.cs - Form11.cs
│   ├── App.config
│   ├── DataSet1.xsd
│   ├── CrystalReport1.rpt
│   ├── CrystalReport2.rpt
│   └── WindowsFormsApplication10.csproj
│
└── fisier_Tabele_final.txt
```

## Running Locally

### Requirements

- Windows
- Visual Studio
- .NET Framework 4.5.1
- Oracle Database
- Oracle Managed Data Access (ODP.NET)
- SAP Crystal Reports runtime for report generation

### Setup

1. Set up an Oracle Database instance.

2. Use `fisier_Tabele_final.txt` to create the database objects, including employee records, payroll calculation triggers and configurable contribution rates.

3. Configure the Oracle database connection in `App.config` according to your local environment.

4. Open `WindowsFormsApplication10.csproj` in Visual Studio.

5. Ensure the required Oracle and Crystal Reports dependencies are available.

6. Build and run the application.

## Purpose

This academic project demonstrates desktop application development using C#, relational database management with Oracle, SQL and PL/SQL programming, automated business logic and employee payroll management.

**Note:** This application is intended for educational purposes. Payroll rates and calculation rules are configurable demonstration values and are not intended for production payroll processing.
