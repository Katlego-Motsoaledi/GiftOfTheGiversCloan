Gift of the Givers Management System

Project Overview

Gift of the Givers Management System is an application created by a group of students. Gift of the Givers Management System is meant to help manage relief operations by putting together disaster incidents, relief centres, volunteers and the work volunteers do.

Gift of the Givers Management System wants to make the planning and coordination of work easier through one central place.

Technologies Used

Programming Language: Kotlin

Framework: ASP.NET Core MVC

.NET Version:.NET 8

Database: Microsoft SQL Server

ORM: Entity Framework Core

Authentication: ASP.NET Core Identity

IDE: Visual Studio

Version Control: Git and GitHub

CI/CD: Azure DevOps Pipelines

Main System Components

1. Incident Management

* Store humanitarian incidents.

* Record incident. Types.

* Track incident locations.

* Record incident start dates.

* Monitor incident statuses.

2. Relief Centre Management

* Keep relief centre information.

* Record centre locations.

* Manage relief centre capacities.

* Link relief centres to incidents.

3. Volunteer Management

* Keep volunteer information.

* Record contact details.

* Maintain volunteer skills and availability.

* Track volunteer registration dates.

* Monitor volunteer statuses.

4. Volunteer Assignments

* Link volunteers to incidents.

* Record assigned roles.

* Track assignment dates.

* Keep volunteer assignment records.

5. User Authentication and Authorisation

* ASP.NET Core Identity integration.

* User authentication.

* Role‑based authorisation.

* Configured. Access‑denied routes.

* Password security requirements.

Database Structure

The SQL Server database contains these tables:

| Table | Description |

|-------|-------------|

| Incidents | Stores humanitarian incident information. |

ReliefCentres | Stores relief centre details. |

Volunteers | Stores volunteer information. |

| VolunteerAssignments | Records volunteer assignments, to incidents. |

The database uses keys foreign keys and indexes to keep data connected and to speed queries.

Installation and Setup

Prerequisites

Make sure the following software is installed:

* Visual Studio 2022 or later.

*.NET 8 SDK.

* Microsoft SQL Server or SQL Server LocalDB.

* SQL Server Management Studio (SSMS).

* Git.

Step 1: Clone the Repository

```bash

git clone https://github.com/Katlego-Motsoaledi/GiftOfTheGiversCloan.git

```

Step 2: Open the Project

1. Open Visual Studio.

2. Select *Open a Project or Solution*.

3. Browse to the folder.

4. Open `gift_of_the_givers.sln`.

Step 3: Configure the Database

Gift of the Givers Management System uses SQL Server LocalDB by default.

The connection string is set in `appsettings.json`:

```json

"ConnectionStrings": {

"DefaultConnection": "Server=(localdb)\\mssqllocaldb;Database=gift_of_the_givers;Trusted_Connection=True;TrustServerCertificate=

}

```

Change the connection string if another SQL Server instance is used.

Step 4: Restore Dependencies

```bash

dotnet restore

```

Step 5: Build the Application

```bash

dotnet build

```

Step 6: Run the Application

```bash

dotnet run

```

Gift of the Givers Management System will start in the ASP.NET Core development environment.

Continuous Integration and Deployment

The repository contains an Azure DevOps pipeline configuration (`azure-pipelines.yml`).

The pipeline is set to:

* Trigger when changes are pushed to the branch.

* Install the.NET 8 SDK.

* Restore NuGet dependencies.

* Build the project.

* Publish the web application.

*. Publish build artifacts.

Version Control

Git and GitHub manage all source code. Allow students to work together.

Repository: https://github.com/Katlego-Motsoaledi/GiftOfTheGiversCloan

Project Purpose

Gift of the Givers Management System shows how software development, database design, authentication, version control and automated builds work together to create a management tool.

Project Status

This is a group project. Gift of the Givers Management System is still being updated.
