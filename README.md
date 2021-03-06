[![Board Status](https://dev.azure.com/lisheard/5be25c07-4c46-4f66-9847-39c5c02a431f/74762dec-b053-413c-941e-bf6d6087d686/_apis/work/boardbadge/c56777d7-1640-4c85-8bc5-17386c66d6c9?columnOptions=1)](https://dev.azure.com/lisheard/5be25c07-4c46-4f66-9847-39c5c02a431f/_boards/board/t/74762dec-b053-413c-941e-bf6d6087d686/Microsoft.RequirementCategory/)

<hr />

# My Driving Team APIs

The DevOps open hack event is designed to foster learning via implementing DevOps practices with a series of challenges.

## Architecture

The application used for this event is a heavily modified and recreated version of the original [My Driving application](https://github.com/Azure-Samples/MyDriving).

The team environment consists of the following:

* Azure App Service for Linux which has four APIs deployed:

  * POI (Trip Points of Interest) - CRUD API written in .Net Core 3.1 for points of interest on trips
  * Trips - CRUD open API written in golang 1.11 for trips connected to the client application
  * UserProfile - CRUD open API written in Node.JS for the users of the client application
    > Note:PATCH/POST operations not functional
  * User-Java - API written in Java with POST and PATCH routes plus swagger docs routes for the users of the client application.
* Mobile Apps - for iOS and Android which will display driving trip data

## Getting Started

To understand each of the components above in more detail, please visit the readme files inside the root folder of each corresponding part of the application.

### Prerequisites

It is useful but not required to have a basic knowledge of the following topics:

* Azure App Services
* Azure Container Registry and Docker
* GitHub, Azure DevOps (formally VSTS) or Jenkins

## Resources

The provisioning of this environment for proctors can be found in the [DevOps Openhack Proctor](https://github.com/Azure-Samples/openhack-devops-proctor) Github repository.
> **Note**: During the Dry Run relevant code can be found in the **openhack_refresh** branch. Post Dry Run these changes will be committed to master.
