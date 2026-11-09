## RaceDay – Part 3

## Project Overview

RaceDay it's a web-based event managements system designed to manage running events. Part-3 MVC focuses on developing an ASP.NET Core MVC web application that connects to the Part 2 API.

The system provides main two types of users: Organiser and Participants. Each user can access to different types features depending on each role.

 These Main Features contains the following:

1. ## Authentications and Navigations

* Users can register and log-in.
* The system maintains the user’s authenticated session.
* Role-based navigation is provided for Organiser and Participant.
* Users can log out securely.
* Unauthenticated users cannot access protected pages.

1. ## Organisers Interface

* Dashboard displaying the event information and enrolments summaries.
* Create, edit and delete the events.
* Manage event categories, including age and distance categories.
* View participants that  enrolled in specific events.
* View of enrolment for statuses.
* Capture participants finishing time and position and record results.
* Upload event banner images.

1. ## Participant Interface

* Their are able to view upcoming events.
* They also able to filter available events.
* View event information and categories.
* They can enroll in events and able to select categories.
* View personal enrolments and enrolment statuses.
* View personal race results.
* Update personal information and profile pictures.

## Technologies that is Used

* C#
* ASP.NET Core MVC
* ASP.NET Core Web API (Part 2)
* HTML
* CSS
* Bootstrap
* Azure Blob Storage
* Docker
* GitHub Actions

## System Architecture

The RaceDay MVC applications communicates with the Part-2 API to retrieve and manage information.

The MVC project application does not directly access the database. All data operations are handled through the Part-2 API.

The application is as follows the Model-View-Controller (MVC) architecture:

* Models: Represent application data.
* Views: Display the user interface.
* Controllers: Handle users requests and communicate with the API.

## Azure Blob Storage Integration

Azure Blob Storage is a integrated through the Part-2 API.

Organisers that can upload event banner images, while Participants they are able to upload their profile pictures.

The MVC application sends images to upload to the Part-2 API. The API handles the storage of images in Azure Blob Storage and  makes them available for display in the application storage.

How to Run the Application Locally

## Requirements

* Visual Studio 2022 or compatible development environments.
* .NET SDK required by the project.
* Access to the Part 2 API.
* SQL Server and required database configuration for the API.

## Steps

1. Clone or download the GitHub repository.
2. Open the MVC project in Visual Studio.
3. Ensure the Part 2 API is running.
4. Check that the API base URL is correctly configured.
5. Build the solution.
6. Run the MVC application.
7. Open the application using the local URL provided by Visual Studio .

## GitHub and CI/CD

GitHub is used for source code management and version control.

GitHub Actions is used to automate the build process.

## The project includes:

* Source code for the MVC applications.
* Dockerfile for containerisation.
* GitHub Actions workflow.
* README documentation.

A minimum of 20-meaningful commits is required for Part 3.

## The Error Handling and User Interface

The applications provide a consistent interface across its pages.

* Navigation is based on user roles.
* Enrolment statuses are displayed using different colours.
* Invalid inputs are handled appropriately.
* The interface uses consistent fonts, colours and spacing.
* Bootstrap is used to support responsive layouts.

## Conclusion

The RaceDay Part-3 project brings the different components of the RaceDay platform together through an ASP.NET Core MVC application.

It provides separate interfaces for Organisers and Participants, integrates with the Part-2 API, support Azure Blob Storages for image uploads, and uses Docker for containerisation.

GitHub and GitHub Actions are used to manage the source code and automate the build process.
