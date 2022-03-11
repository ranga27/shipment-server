# Shipment Client API

## Overview
This Client API is a bare-bones vanilla Node.js module without any frameworks. I haven't used any third-party libraries and thus have minimal abstraction. It helps to focus on the core functionalities of the API using bare minimum Node.js modules. 

## Goal
The API's primary goal is to expose interfaces, functions and methods that aim to achieve the following:
* Managing shipments and packages - simple CRUD
* Reporting associated data with the shipments and packages

## Getting Started
- Install Node.js runtime for your environment from https://nodejs.org/en/download/
- You can also install it through package managers like Homebrew (Mac) and Chocolatey (Windows).
- Clone this project and navigate to the home directory

## Available Functions:
- Shipment & Package Management
  - Create Shipment
  - Create Package
  - Get All Shipments
  - Get Shipments by ID
  - Get Packages by ID
  - Update Shipment
  - Add Package to a Shipment
  - Remove a Package from a Shipment
- Reporting
  - Shipments & Packages associated with a specific Supplier <-> Buyer pair
  - Carbon emissions for a specific supplier
  - The most efficient supplier for carbon emissions

## API endpoints 
These endpoints allow you to handle the management of shipments packages and report on their attributes 

## Constraints
- No backend DB is used. Instead, I have used the filesystem is used for ease of simplicity.
- Creation of empty shipments is not allowed. To create a shipment, adding at least one existing package is mandatory. Hence it would be best to create a package before creating a shipment.

## Test Data
I have provided Test data for testing the functionality of individual modules.

## Assumptions
- Shipment & Package Data is available in JSON format
- Each shipment & each package are associated with a unique ID
- For Train Packages distances, distance are mutually exclusive since it's associated with a package and not shipment.

## Backlog/Roadmap
- Updating an existing package within a shipment
- Updating vehicle type in a shipment & associated validations 
- Setting up the HTTP server and the REST API 

## TODO
- [ ] Error Handling
- [ ] Improve Function Documentation