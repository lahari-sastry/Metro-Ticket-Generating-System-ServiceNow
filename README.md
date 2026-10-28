# Metro Ticket Booking and QR Ticket Generation using ServiceNow

## Project Overview

**Metro Ticket Booking and QR Ticket Generation** is a ServiceNow-based
digital ticketing system designed to simplify and automate the metro
ticket booking process.

The project provides a user-friendly ServiceNow Service Portal form
where commuters can enter their journey details, select metro stations,
choose the journey type, specify the number of passengers, and generate
a digital metro ticket.

The system uses ServiceNow configuration, Catalog Items, Catalog
Variables, Catalog Client Scripts, Catalog UI Policies, and scripting to
automate important parts of the ticket-booking process such as fare
calculation and QR ticket generation.

------------------------------------------------------------------------

## Objectives

The main objectives of the project are:

-   Digitize the metro ticket booking process.
-   Reduce the dependency on manual ticket booking.
-   Allow users to select source and destination metro stations easily.
-   Support single and return journey options.
-   Calculate the applicable fare automatically.
-   Generate a digital metro ticket with a QR code.
-   Provide a simple ServiceNow Service Portal interface.
-   Automate ticket-related processing using ServiceNow scripting and
    configuration.

------------------------------------------------------------------------

## Key Features

### 1. Metro Station Management

A dedicated **Metro Station Detail** table is used to maintain metro
station information.

The project includes station records that can be used while booking a
ticket. This allows the booking form to provide station choices for the
user's journey.

### 2. Service Catalog Item

A ServiceNow Service Catalog Item named:

> **Book a Metro Ticket**

is used as the main entry point for the ticket-booking process.

The Catalog Item contains the variables required to collect journey and
passenger information.

### 3. Journey Details

The booking form allows the user to provide journey-related information
such as:

-   Source station
-   Destination station
-   Journey type
-   Number of passengers

### 4. Automatic Fare Calculation

The project uses a **Catalog Client Script** to automatically calculate
the ticket fare based on the selected booking information.

This reduces manual calculation and provides the fare directly within
the booking process.

### 5. Catalog UI Policy

A **Catalog UI Policy** is used to control the dynamic behavior of
fields in the Service Catalog form.

This helps make the form more user-friendly by controlling field
behavior based on the booking information.

### 6. QR Ticket Generation

After the booking process, the system generates a digital metro ticket
containing a **QR code**.

The QR ticket provides a digital representation of the generated ticket
and can be used as part of the ticket verification process.

### 7. Service Portal Interface

The project is accessible through a ServiceNow Service Portal interface.

The commuter can enter the required details through the **Book a Metro
Ticket** form instead of depending on a manual ticketing process.

------------------------------------------------------------------------

## Technology Stack

  -----------------------------------------------------------------------
  Technology                          Purpose
  ----------------------------------- -----------------------------------
  **ServiceNow**                      Main development and
                                      service-management platform

  **Service Catalog**                 Metro ticket booking interface

  **Service Portal**                  User-facing booking form

  **Catalog Client Scripts**          Fare calculation and ticket-related
                                      client-side automation

  **Catalog UI Policies**             Dynamic field behavior

  **ServiceNow Scripting**            Automation and ticket generation
                                      logic

  **QR Code**                         Digital metro ticket representation
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## System Workflow

The overall workflow of the project can be summarized as:

``` text
User
  |
  v
ServiceNow Service Portal
  |
  v
Book a Metro Ticket
  |
  v
Enter Journey Details
  |
  +----------------------+
  |                      |
  v                      v
Select Stations      Select Journey Type
  |                      |
  +----------+-----------+
             |
             v
     Enter Passenger Count
             |
             v
      Automatic Fare
        Calculation
             |
             v
       Submit Request
             |
             v
      Ticket Generation
             |
             v
       QR Code Ticket
```

------------------------------------------------------------------------

## Main ServiceNow Components

### Metro Station Detail Table

The project contains a Metro Station Detail table for maintaining
station information.

The station data is used by the booking form to provide source and
destination station selections.

### Catalog Item

The primary Catalog Item is:

**Book a Metro Ticket**

It acts as the interface through which users submit metro ticket
requests.

### Catalog Variables

The Catalog Item uses variables to collect the information required for
a metro ticket request, including station, journey, and passenger
details.

### Catalog Client Scripts

Client-side scripts are used to automate form behavior.

Two important scripting components demonstrated in the project are:

-   **Fare Auto-Calculation Client Script**
-   **OR Generation Client Script**

These scripts help automate the ticket-booking process.

### Catalog UI Policy

The Catalog UI Policy controls the behavior and visibility/state of
relevant fields on the booking form.

------------------------------------------------------------------------

## Example Booking Flow

A typical booking can follow this sequence:

1.  Open the **Book a Metro Ticket** Service Catalog Item.
2.  Select the source station.
3.  Select the destination station.
4.  Select the journey type.
5.  Enter the number of passengers.
6.  Allow the system to calculate the fare automatically.
7.  Submit the ticket request.
8.  Generate the digital metro ticket.
9.  Display the generated QR ticket.

------------------------------------------------------------------------

## Project Screens / Demonstrated Outputs

The project demonstration includes the following major outputs:

1.  **Metro Station Table and Records**
2.  **Service Catalog Item and Variables**
3.  **Fare Auto-Calculation Configuration**
4.  **Catalog UI Policy**
5.  **QR Generation Configuration**
6.  **Metro Ticket Request Form**
7.  **Automatic Fare Result**
8.  **Generated Metro QR Ticket**

These outputs demonstrate the configuration and working flow of the
ServiceNow metro ticketing system.

------------------------------------------------------------------------

## Functional Requirements

  -----------------------------------------------------------------------
  ID                      Functional Requirement  Demonstrated Through
  ----------------------- ----------------------- -----------------------
  FR-1                    Ticket Request          Service Catalog Item
                          Submission              and Metro Ticket Form

  FR-2                    Station Data and        Metro Station Table and
                          Variables               Catalog Variables

  FR-3                    Automatic Fare          Client Script and
                          Calculation             Booking Form

  FR-4                    Dynamic Field Behavior  Catalog UI Policy and
                                                  Form

  FR-5                    QR Ticket Generation    QR Generation Script
                                                  and Generated Ticket
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## Advantages

-   Reduces manual effort in metro ticket booking.
-   Provides a digital alternative to conventional ticket booking.
-   Automates fare calculation.
-   Provides a structured Service Catalog-based booking process.
-   Generates a digital QR ticket.
-   Provides a simple user-facing Service Portal interface.
-   Uses ServiceNow configuration and automation capabilities.

------------------------------------------------------------------------

## Future Enhancements

The project can be extended with additional features such as:

-   Online payment integration.
-   Real-time metro station and route information.
-   QR code scanning and validation.
-   Ticket cancellation and refund management.
-   Ticket history for commuters.
-   Email or SMS ticket notifications.
-   Mobile-friendly enhancements.
-   Integration with actual metro fare and station APIs.
-   Admin dashboard for monitoring ticket requests.

------------------------------------------------------------------------

## Project Demo

**Google Drive Demo Video:**

[View Metro Ticketing Project
Demo](https://drive.google.com/file/d/1ItrD82QcwvmBkayxnWmWrdD-3kSEhMLe/view?usp=drivesdk)

------------------------------------------------------------------------

## Project Summary

The **Metro Ticket Booking and QR Ticket Generation using ServiceNow**
project demonstrates how ServiceNow can be used to digitize and automate
a metro ticketing workflow.

By combining Service Catalog configuration, station data, Catalog
Variables, Client Scripts, UI Policies, and QR ticket generation, the
system provides a structured digital process from entering journey
details to generating a metro QR ticket.

------------------------------------------------------------------------

## Author

**Jonnalagadda Sai Sri Poornima Lahari**

B.Tech -- Artificial Intelligence & Data Science
