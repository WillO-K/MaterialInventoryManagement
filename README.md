# MaterialInventoryManagement

## Background
EOS Lighting requires a more streamlined way of managing materials inventory; something that isn't a couple of complicated Excel sheets that require manually editing each time, as the materials list grows larger as more products are added to the repertoire. The idea that I had to manage this is create an operational normalized database with tables for materials, suppliers, purchase orders, etc... And then create some sort of "front-end" app to allow records to be modified without, for a start, requiring knowledge of SQL. The "front-end" should also touch more than just 1 table when an action is performed too (e.g, when a new purchase order is fulfilled by the supplier, the system updates the purchase order table to _Status: Completed_ and updates the materials table to increase quantity. I use the phrase "front-end" loosely; I'm not a full-stack developer, I'm not a web dev, and I'm not a software engineer. I'm still a Data/BI analyst, so this front end could end up being or looking like anything. 

## Goals
* Create a database with several tables to make managing materials inventory easier/streamlined.
* Create a (broadly speaking) front-end for non-SQL users
* Look to create some procedures in database that are actioned when something specific is done in the front-end

## Tools
* MySQL/MariaDB - We've used this in a previous project, and is reliable and simple enough for this use case.
* Debian - The database and front-end will run off a server running Debian.
* TBC
