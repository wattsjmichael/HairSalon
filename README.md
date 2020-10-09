# Eau Claire's Salon

#### Eau Claire's Salon allows an user to input Stylist and Clients and associate the data

#### By Michael Watts

## Description

Eau Claire's Salon is a C#/CSHTML Website that allows to create new stylists and clients and associate the clients to the stylists. 

## Setup/Installation Requirements

## MySQL Workbench Schema Setup:
1. Open [MySql Workbench](https://www.mysql.com/products/workbench/) and connect to Local instance
2. Create a new sql tab by clicking the upper left icon: 'Create A New SQL Tab for Executing Queries'
3. Copy and paste the following code into "Query" and "Run":
---
### **Copy The Following Text**
CREATE DATABASE `ichael_watts` /*!40100 DEFAULT CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci */ /*!80016 DEFAULT ENCRYPTION='N' */;
USE ichael_watts;
CREATE TABLE `clients` (
  `ClientId` int NOT NULL AUTO_INCREMENT,
  `ClientName` varchar(255) DEFAULT NULL,
  `StylistId` int DEFAULT '0',
  PRIMARY KEY (`ClientId`)
) ENGINE=InnoDB AUTO_INCREMENT=12 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
CREATE TABLE `stylists` (
  `StylistId` int NOT NULL AUTO_INCREMENT,
  `Name` varchar(255) DEFAULT NULL,
  `Speciality` varchar(255) DEFAULT NULL,
  PRIMARY KEY (`StylistId`)
) ENGINE=InnoDB AUTO_INCREMENT=8 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;

## Website Setup:
* Download or Clone project from Github repository.
* Open a terminal within HairSalon folder within main project directory.
* Use Command, type in 'dotnet build'.
* After build, run the program with 'dotnet run' in the terminal.
* If you don't have it already, create a "appsettings.json" file in the "HairSalon" directory and Insert the code below with your user name and password for MySQL: 

> {
>  "ConnectionStrings": {
>      "DefaultConnection": "Server=localhost;Port=3306;database=michael_watts;uid={YOUR USERNAME};pwd={YOUR USERNAME}"
>  }
>}
## Known Bugs

No Known Bugs

## Support and contact details

https://github.com/wattsjmichael

## Technologies Used

C#, LINQ, Entity Framework Core, MVCTest, MySql, CSHTML, CSS, Bootstrap and Markdown.

## Link To Active Site:
Not Applicable

### License

This software is licensed under the MIT license.

Copyright (c) 2020 **Michael Watts** - _Eau Claire's Salon_
