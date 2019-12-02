# Exercise 0402 - Fleet Manager

You own a company where salespeople regularly run customer visits. They use company cars to drive around but you have troubles with keeping track of when the cars are home and when they are not. So you have decided to create a small piece of software, where you can register when the cars are home.

The *functional requirements* for your application are as follows:
1. Insert a car with the properties of brand and model into the table
1. Delete a car from the table
1. View a list of cars that are away.
1. View a list of available cars.
1. Select a car and mark it as in use.
   1. It should *not* be possible to mark a car that already is in use.
1. Select a car and mark it as available.
   1. It should *only* be possible to mark a car that is in use.

The *non-functional requirements* are:
1. Car data must be stored in a sql server database.
1. You have to create the solution with the .NET Framework and use ADO.NET for data access.
1. The user interface must be text-based, so you need to implement the solution as a console application.


You can create tables yourself to store data, but the script below creates a table that should be sufficient to solve the task.

```
CREATE TABLE [dbo].[Cars] (
    [Id] INT PRIMARY KEY NOT NULL,
    [Brand] NVARCHAR (50) NULL,
    [Model] NVARCHAR (50) NULL,
    [Home] BIT NULL
);
```
