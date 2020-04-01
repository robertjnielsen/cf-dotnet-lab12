# Databases And ERDs

Code Fellows 401 .NET Course - Lab 12  
_Author: [Robert James Nielsen](https://github.com/robertjnielsen)_

## Overview

### ERD Explanation
#### Table: Location
Each Location has properties to determine its address, etc. It also has a Primary Key as an ID. Location also navigates to the LocationRooms table to be used as a Join Table with Payload.

#### Table: LocationRooms
LocationRooms is a Join Table with Payload. It joins our Location model, and our Room model, and holds an enum for floor number, as well as a property for whether there are exterior windows or not. It navigates to both Location, and Room.

#### Table: Room
Each Room holds properties for information about the Room such as bedrooms, Price, etc. It has a Primary Key of ID, and navigates to LocationRooms and RoomAmenities.

#### Table: RoomAmenities
The RoomAmenities table is a Pure Join Table for the Room model and The Amenities model.

#### Table: Amenities
The Amenities table holds a Primary Key of ID, as well as several boolean properties to determine which amenities are available in a given room. It navigates to the RoomAmenities table.

## Getting Started

## Visuals

#### Entity Relationship Diagram
![ERD](/Assets/Images/Lab12ERD.png)

## Change Log
