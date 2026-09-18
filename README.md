# Smart India Hackathon Workshop

## Date:

18-09-2026

## Register Number:

212224040279

## Name:
RIYAZ M

---

# Problem Title

**SIH 1710: Enhancing Navigation for Railway Station Facilities and Locations**

# Problem Description

Railway stations are complex environments containing various facilities such as platforms, ticket counters, restrooms, waiting halls, food courts, lifts, escalators, exits and parking areas. Passengers, especially first-time visitors, elderly people and passengers with disabilities, may face difficulties in locating these facilities quickly.

The problem is to develop a comprehensive and user-friendly navigation system that helps passengers locate railway station facilities and destinations efficiently. The system should provide interactive maps, real-time directions, accessibility options and voice-guided navigation.

The proposed solution provides navigation through both mobile devices and digital kiosks. It helps passengers select a destination and receive suitable step-by-step directions within the railway station.

# Problem Creator's Organization

**Ministry of Railway**

---

# Idea

## RailWayNav – Smart Indoor Railway Navigation System

RailWayNav is a smart indoor railway station navigation system designed to help passengers easily find platforms, facilities and important locations inside railway stations.

The system provides an interactive station map through a mobile application and digital kiosks. Passengers can search for a destination such as a platform, restroom, ticket counter, waiting hall, food court, lift, escalator or exit.

After selecting the destination, the system calculates a suitable route and provides step-by-step navigation instructions.

### Key Features

* Interactive railway station map
* Indoor route navigation
* Platform and facility search
* Step-by-step directions
* Wheelchair-accessible route
* Lift and ramp-based navigation
* Voice-guided navigation
* Emergency exit navigation
* Digital kiosk support
* Multi-language support
* Station information updates
* Temporary facility and route closure updates

---

# Proposed Solution

The proposed system consists of a mobile application, digital kiosks, navigation engine, station database and administrator dashboard.

The passenger can use the mobile application or a digital kiosk to search for a destination inside the railway station.

The navigation engine receives the passenger's current location and selected destination. It then calculates an appropriate route using station map data.

If accessibility mode is enabled, the system avoids stairs and provides routes using lifts and ramps wherever available.

Voice guidance can provide instructions to visually impaired passengers. Railway administrators can update station maps, facility locations and temporary closures through the administration dashboard.

## Proposed Solution Architecture

```text
                    ┌───────────────────────┐
                    │       PASSENGER       │
                    │                       │
                    │   Mobile App / Kiosk  │
                    └───────────┬───────────┘
                                │
                                ▼
                    ┌───────────────────────┐
                    │     USER INTERFACE    │
                    │                       │
                    │ Map | Search | Voice  │
                    │ Accessibility Mode    │
                    └───────────┬───────────┘
                                │
                                ▼
                    ┌───────────────────────┐
                    │   NAVIGATION ENGINE   │
                    │                       │
                    │ Route Calculation     │
                    │ Indoor Positioning    │
                    │ Accessibility Route   │
                    └───────────┬───────────┘
                                │
                                ▼
              ┌─────────────────────────────────┐
              │       STATION DATA SERVER       │
              │                                 │
              │ Station Map                     │
              │ Facility Locations              │
              │ Platform Information            │
              │ Navigation Data                 │
              └───────────────┬─────────────────┘
                              │
                              ▼
                    ┌───────────────────────┐
                    │   ADMIN DASHBOARD      │
                    │                       │
                    │ Update Station Map     │
                    │ Manage Facilities     │
                    │ Update Closures        │
                    │ Monitor System         │
                    └───────────────────────┘
```

## Working Process

1. The passenger opens the RailWayNav mobile application or uses a digital kiosk.
2. The system identifies the passenger's approximate indoor location using available positioning technologies.
3. The passenger searches for a destination.
4. The system retrieves the selected destination from the station database.
5. The navigation engine calculates a suitable route.
6. The route is displayed on the interactive station map.
7. Step-by-step instructions are provided to the passenger.
8. Voice guidance can be enabled for visually impaired passengers.
9. Accessibility mode provides routes using lifts and ramps while avoiding stairs.
10. Administrators can update station information whenever facilities or routes change.

---

# Use Cases

## Use Case Diagram

```text
                         ┌─────────────────────────┐
                         │     RailWayNav System   │
                         └─────────────────────────┘
                              /      |       \
                             /       |        \
                            ▼        ▼         ▼
                     Search Facility  View Map  Get Directions
                            │           │          │
                            │           │          │
                     ┌──────┴───────────┴──────────┴──────┐
                     │                                    │
                     ▼                                    ▼
              Accessibility Mode                   Voice Navigation
                     │                                    │
                     └────────────────┬───────────────────┘
                                      │
                                      ▼
                                  Passenger


                      Administrator
                           │
             ┌─────────────┼─────────────┐
             ▼             ▼             ▼
        Update Map   Manage Facilities  Update Closures
             │             │             │
             └─────────────┼─────────────┘
                           ▼
                     Monitor System
```

## Passenger Use Cases

### 1. Search Facility

The passenger can search for facilities such as platforms, ticket counters, restrooms, waiting halls, food courts and exits.

### 2. View Station Map

The passenger can view an interactive map of the railway station and identify different facilities and locations.

### 3. Get Directions

The system calculates a route from the passenger's current location to the selected destination.

### 4. Accessibility Navigation

Passengers can enable accessibility mode to receive routes that prioritize lifts, ramps and accessible pathways.

### 5. Voice Navigation

The system provides voice instructions for passengers who require audio-based navigation.

### 6. Emergency Navigation

The system helps passengers locate emergency exits, medical facilities, help desks and other important locations.

## Administrator Use Cases

### 1. Update Station Map

Administrators can update the station layout and navigation information.

### 2. Manage Facilities

Administrators can add, modify or remove facility information.

### 3. Update Temporary Closures

Administrators can mark facilities or routes as temporarily unavailable.

### 4. Monitor System

Administrators can monitor station navigation data and system status.

---

# Technology Stack

## Frontend

* React.js
* React Native
* HTML5
* CSS3
* JavaScript

## Map and Navigation

* Three.js
* Leaflet
* Graph-based route calculation
* Indoor positioning technologies

## Backend

* Node.js
* Express.js
* REST API

## Database

* MongoDB

The database stores:

* Station information
* Platform information
* Facility locations
* Navigation nodes
* Accessibility information
* Temporary closures

## Additional Technologies

* Web Speech API for voice navigation
* JWT for administrator authentication
* Git for version control
* GitHub for project management
* Figma for UI/UX design

---

# Dependencies

## Software Dependencies

* Node.js
* npm
* React.js
* React Native
* Express.js
* MongoDB
* Three.js
* Leaflet
* Git
* GitHub
* Modern web browser

## Hardware Dependencies

* Smartphone or tablet
* Touch-screen digital kiosk
* Server or cloud infrastructure
* Wi-Fi/Bluetooth infrastructure for indoor positioning where available

## Data Dependencies

* Railway station floor maps
* Platform information
* Facility locations
* Entrance and exit locations
* Lift and ramp locations
* Accessibility information
* Temporary closure information

## External Services

* Railway information APIs, where officially available
* Map services where required
* Text-to-speech services
* Notification services

---

# Advantages

* Reduces passenger confusion inside railway stations.
* Helps passengers locate platforms and facilities easily.
* Provides accessible routes for passengers with disabilities.
* Supports visually impaired passengers through voice guidance.
* Helps passengers save time while finding destinations.
* Provides navigation through both mobile applications and digital kiosks.
* Allows railway authorities to update station information.
* Helps reduce unnecessary passenger movement inside stations.
* Provides emergency route information.

---

# Expected Outcome

The proposed RailWayNav system will provide a simple and efficient way for passengers to navigate railway stations.

Passengers will be able to search for facilities, view interactive maps, receive step-by-step directions and select accessibility-friendly routes. Voice navigation will improve accessibility for visually impaired passengers.

The administrator dashboard will allow railway authorities to maintain accurate station information and update changes in facilities, routes and temporary closures.

---

# Future Enhancements

* AI-based passenger flow analysis
* AR-based navigation using smartphone cameras
* Real-time crowd density information
* Integration with train arrival and departure information
* Smart wearable device support
* More Indian regional languages
* Predictive route suggestions during high passenger traffic
* Integration with official railway applications and services

---

# Conclusion

RailWayNav is a smart indoor navigation solution for railway stations that combines interactive maps, route calculation, accessibility features, voice guidance and digital kiosks.

The system aims to make railway stations easier to navigate by providing passengers with accurate and accessible directions to platforms and facilities. The administrator dashboard also enables railway authorities to maintain and update station information efficiently.
