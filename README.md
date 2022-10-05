# DevOpti
Empty "Optimizely CMS 12" project, inited using "epi-cms-empty" template.
An empty site for quick experiments

**Database**

Create new empty database in MS SQL Server: 
```
CREATE DATABASE [<YOUR_DATABASE_NAME_HERE>]
GO
```
Next user:
1. Use your Windows login with "Trused Connection" option.
or
2. Create a new user with "SQL Server auth" in MS SQL Server and assign your newly created database to him via settings page "General", dropdown "Default database" and add mapping via settings page "User Mapping" -> select your db and assing "db_owner" role. For the development stage "db_owner" role is an applicable option. Also don't forget to update connection string in "appsettings.json" file with new credentials.

Build and run the project: Optimizely CNS 12 will create all necessary tables in the database and opens the page to create an administrator account. Once the admin account is created, this functionality will be disabled.
Thus no need to store a backup of an empty database and a new site for experiments can be created and launched almost immediately.