# Sasto Tickets Web-SDK Integration

## Introduction

The Web SDK allows you to integrate the services provided by Sasto Tickets into your web application. This document provided an overview of the SDK, how to initialize it using a link with encoded parameters, and outlines the flight booking and ticketing workflow supported bu SDK.

## Initialization

To initializxe the Web SDK, you need to open a specic URL with additional parameters encoded in Base64. These parameters will provide necessary data for the SDK to function

The SDK initialization URL should follow the format:

    https://demo.sastotickets.com/?data=<base64_encoded_parameters>

### Parameters

The parameters should be encoded in Base64 format and contain the necessary information for the SDK. Here's an example of the encoded parameter structure:

    {
        "mobile" : "9801234567",
        "name": "Demo User",
        "email":"demo.user@test.com"
    }

Encode the entire JSON structure in Base64, including the access token, and replace `<base64_encoded_parameters>` in the initialization URL with the actual encoded parameters.


## Flight Booking & Ticketing Workflow

The flight booking and ticketing workflow will be handled by the SDK. Here's the actions involved:

    Step 1. Flight Search
    Step 2. Availability
    Step 3. Reservation
    Step 4. Payment
    Step 5. Issue Ticket


<div style="background-color: #E2F0F7; padding:10px; border-radius:5px "><b>Note:</b> All of the above actions be handled by our Web SDK.</div>

That's it! With the SDK integration, the flight booking and ticketing actions will be seamlessly handled within your web application.

