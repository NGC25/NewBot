
Space Bot API Investigation Sheet
**Total Marks: 30**
**Part 1: Collect Required API Documentation**
This investigation sheet helps you gather key technical information from the three
APIs required for the Space Bot project: **Webex Messaging API**, **ISS Current
Location API**, and a **Geocoding API** (LocationIQ or Mapbox or other), plus the
Python time module.
---
Webex api: MDIzZGJmN2QtMDFkOS00MDhkLWEwNzQtZjMzYWMxN2FjNjhjYzkwZWY3MTItNjBj_P0A1_bdd2aed2-da17-481d-bd6f-b43037ee90b7

| Criteria | Details |
|---------|---------|
| API Base URL | https://webexapis.com/v1//
| Authentication Method | `bearer token` |
| Endpoint to list rooms | `/rooms` |
| Endpoint to get messages | `/messages` |
| Endpoint to send message | `/messages ` |
| Required headers | `__Aurthorisation,Bearer token, content-type, Json` |
| Sample full GET or POST request | `{
    "items": [
        {
            "id": "Y2lzY29zcGFyazovL3VybjpURUFNOnVzLXdlc3QtMl9yL1JPT00vMzMzM2IwNjAtYWYyZC0xMWYwLTllMTItYTdlMDg1ODg0Nzhl",
            "title": "BOT",
            "type": "group",
            "isLocked": false,
            "lastActivity": "2025-10-22T10:15:00.228Z",
            "creatorId": "Y2lzY29zcGFyazovL3VzL1BFT1BMRS8yNzg0YTk3NS01MjRkLTQ5MzAtYjEzZi1lNmRkZDc2NDUyY2U",
            "created": "2025-10-22T09:55:11.590Z",
            "ownerId": "Y2lzY29zcGFyazovL3VzL09SR0FOSVpBVElPTi9iZGQyYWVkMi1kYTE3LTQ4MWQtYmQ2Zi1iNDMwMzdlZTkwYjc",
            "isPublic": false,
            "isReadOnly": false
        },
        {
            "id": "Y2lzY29zcGFyazovL3VybjpURUFNOnVzLXdlc3QtMl9yL1JPT00vODgxMjNjNDAtYTQyZi0xMWYwLWEzYTQtNzczM2UyOGI1MWIw",
            "title": "Naesha's space",
            "type": "group",
            "isLocked": false,
            "lastActivity": "2025-10-08T10:14:10.180Z",
            "creatorId": "Y2lzY29zcGFyazovL3VzL1BFT1BMRS8yNzg0YTk3NS01MjRkLTQ5MzAtYjEzZi1lNmRkZDc2NDUyY2U",
            "created": "2025-10-08T10:14:10.180Z",
            "ownerId": "Y2lzY29zcGFyazovL3VzL09SR0FOSVpBVElPTi9iZGQyYWVkMi1kYTE3LTQ4MWQtYmQ2Zi1iNDMwMzdlZTkwYjc",
            "isPublic": false,
            "isReadOnly": false
        }
    ]
}
` |
---
## Section 2: ISS Current Location API (3 marks)
| Criteria | Details |
|---------|---------|
| API Base URL | `https://api.openweathermap.org/` |
| Endpoint for current ISS location | `/data/2.5/weatherlondon` |
| Sample response format (example JSON) |
```
{
    "coord": {
        "lon": 21,
        "lat": 12
    },
    "weather": [
        {
            "id": 804,
            "main": "Clouds",
            "description": "overcast clouds",
            "icon": "04d"
        }
    ],
    "base": "stations",
    "main": {
        "temp": 308.3,
        "feels_like": 305.95,
        "temp_min": 308.3,
        "temp_max": 308.3,
        "pressure": 1006,
        "humidity": 16,
        "sea_level": 1006,
        "grnd_level": 950
    },
    "visibility": 10000,
    "wind": {
        "speed": 1.56,
        "deg": 130,
        "gust": 1.81
    },
    "clouds": {
        "all": 100
    },
    "dt": 1761834679,
    "sys": {
        "country": "TD",
        "sunrise": 1761798483,
        "sunset": 1761840665
    },
    "timezone": 3600,
    "id": 242048,
    "name": "Salamat Region",
    "cod": 200
}
```
|
---
## Section 3: Geocoding API (LocationIQ or Mapbox or other) (6 marks)
| Criteria | Details |
|---------|---------|
| Provider used (circle one) | **LocationIQ / Mapbox/ other -provide detail** |
| API Base URL | `_______________________________` |
| Endpoint for reverse geocoding | `_______________________________` |
| Authentication method | `_______________________________` |
| Required query parameters | `_______________________________` |
| Sample request with latitude/longitude | `_______________________________` |
| Sample JSON response (formatted example) |
```
```
|
---
## 🚀 Section 4: Epoch to Human Time Conversion (Python time module) (2 marks)
| Criteria | Details |
|---------|---------|
| Library used | `_______________________________` |
| Function used to convert epoch | `_______________________________` |
| Sample code to convert timestamp |
```
```
|
| Output (human-readable time) | `_______________________________` |
---
## 🚀 Section 5: Web Architecture & MVC Design Pattern (12 marks)
### 🚀 Web Architecture – Client-Server Model
- **Client**:
- **Server**:
- (Explain the communication between them & include a block diagram )
### 🚀 RESTful API Usage
-
-
-
### 🚀 MVC Pattern in Space Bot
| Component | Description |
|------------|-------------|
| **Model** | |
| **View** | |
| **Controller** | |
#### Example:
- Model:
- View:
- Controller:
---
### 🚀 Notes
- Use official documentation for accuracy (e.g. developer.webex.com, locationiq.com
or Mapbox, open-notify.org or other ISS API).
- Be prepared to explain your findings to your instructor or demo how you retrieved
them using tools like Postman, Curl, or Python scripts.
---
### Total: /30


To complete this Space Bot API Investigation Sheet, follow the steps below section by section, ensuring you extract accurate data from the official API documentation of each service. This will help you understand the APIs used in your Space Bot project, and be prepared for integration and testing.
# NewBot
