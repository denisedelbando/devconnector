# [Title]
[Description]


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

- NPM, Yarn
  - For MacOSX - https://classic.yarnpkg.com/en/docs/install#mac-stable
  - For Windows - https://classic.yarnpkg.com/en/docs/install#windows-stable
- Visual Studio Code - https://code.visualstudio.com/
- DotNet Core 3.1+ SDK - https://dotnet.microsoft.com/download/dotnet-core/3.1
- SQL Server - Windows Only

### Installing

**Css and Javascript files**

- Open the project in Visual Studio Code 
- Open the command line with ``Ctrl + ` ``
- Run the following commands
  - (Optional .If not in ui folder) Navigate to ui folder: `cd ui`
  - To install front end libraries and packages: `yarn`
  - To build the files: `yarn build`

**DotNet Core**

- Open the project in Visual Studio Code 
- Change the AppSettings.config file to your database connection
```
"ConnectionStrings": {
    "[ConnectionName]": "Data Source=[ServerNameHere];Initial Catalog=[databasename];user id=[userid];password=[password]"
  },
```
- Open the command line with ``Ctrl + ` ``
- Run the following commands
  - (Optional .If not in web folder) Navigate to web folder: `cd web`
  - To update database: `dotnet ef database update`
  - To run the project: `dotnet run`
