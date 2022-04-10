# Pierre's Treats

#### By _**Phil Curran**_

#### An MVC web app that manages relationships between two different datasets.

## Technologies Used

* C#
* .Net 5.0
* MySql 8.0 & MySql Workbench
* Bulma CSS

## Description

An MVC web app that manages relationships between two different datasets.  Create a Treat profile, a Flavor Profile, and manage the relationship between the Treats and different flavors of treats.

## Setup/Installation Requirements

* Install or Update MySql to version 8.0
* Install or Update .net to 5.0
* Install or Update dotnet-ef to version 5.0
* Download repo: link
* Create an <code>appsettings.json</code> file in your root directory and add the following code:

```json
{
  "ConnectionStrings": {
    "ConnectionString": "server=localhost;user id=[ user id ];password=[ user password ];port=3306;database=[ database name ];"
  }
}
```
* Update the appsettings.json file by replacing the <code>[ user id ]</code>, <code>[ user password ]</code>, and <code>[ database name ]</code> above with your MySql user id, password, and desired database name.
* Navigate to the root directory of the project
* Create an initial database migration for the project: <code>dotnet ef migrations add InitialCreate</code>
* Update the database: <code>dotnet ef database update</code>
* Use MySql Workbench to verify that the database table has been created
* Install dependencies: dotnet restore
* Build & check for errors: dotnet build
* Run the project: dotnet watch run

## Known Bugs

* View / Treats / Edit causes an error; it looks like it can't access the list of flavors to populate the dropdown menu to edit flavor.

## Contact Me

Let me know what you think! pecurran@hotmail.com

## License

Copyright (c) 2022 / Phil Curran