# CarRent is an app for managing car rental companies.

# Requirements:
.Net 6.0,
SQL Server 2017+


# How to prepare the application:
1. Clone repository 
2. Make migration
a) Open Terminal in project main folder "carrent"
b) run command: dotnet ef database update InitialMigration --project CarRent.DAL -s CarRent -c ApplicationDbContext
3. Run application


# Roles Permissions:
User: (default*)
1. LogIn
2. Explore Cars to rent
3. Check own current and historical rentals

Employee:
1. Everything from User
2. Add new cars
3. Check all active rentals

Administrator*:
1. Everything from User
2. Manage all users roles
3. Adding roles


*The very first registered user will be the administrator
