
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
| Provider used (circle one) | **LocationIQ ** |
| API Base URL | `https://us1.locationiq.com/` |
| Endpoint for reverse geocoding | `/v1/reverse` |
| Authentication method | `access token` |
| Required query parameters | `?key=pk.6cf6740e8ca0f1c50b4985d3a68bc824&` |
| Sample request with latitude/longitude | `https://us1.locationiq.com?key=pk.6cf6740e8ca0f1c50b4985d3a68bc824&lat=50.172&lon=-1.852&format=json` |
| Sample JSON response (formatted example) |
```
{
    "place_id": "274040031",
    "licence": "https://locationiq.com/attribution",
    "osm_type": "node",
    "osm_id": "7817017136",
    "lat": "51.5074062",
    "lon": "-0.1276915",
    "display_name": "Mileage Central Point of London Plaque, Charing Cross, Seven Dials, Waterloo, City of Westminster, Greater London, England, WC2N 5DX, United Kingdom",
    "address": {
        "memorial": "Mileage Central Point of London Plaque",
        "road": "Charing Cross",
        "neighbourhood": "Seven Dials",
        "suburb": "Waterloo",
        "city": "City of Westminster",
        "state_district": "Greater London",
        "state": "England",
        "postcode": "WC2N 5DX",
        "country": "United Kingdom",
        "country_code": "gb"
    },
    "boundingbox": [
        "51.5073562",
        "51.5074562",
        "-0.1277415",
        "-0.1276415"
    ]
}
```
|
---
## 🚀 Section 4: Epoch to Human Time Conversion (Python time module) (2 marks)
| Criteria | Details |
|---------|---------|
| Library used | `import time` |
| Function used to convert epoch | `time.ctime()` |
| Sample code to convert timestamp |
```
import time 

Epochtime = 30000 
convert = time.ctime(Epochtime) 


print(convert)

```
|
| Output (human-readable time) | `Thu Jan  1 08:20:00 1970` |
---
## 🚀 Section 5: Web Architecture & MVC Design Pattern (12 marks)
### 🚀 Web Architecture – Client-Server Model
- **Client**: to make changes it must talk to the server buy sending requests
- **Server**: processes the request and sends back infomation
- <img width="1066" height="525" alt="image" src="https://github.com/user-attachments/assets/e00dd964-7483-4ad7-ad27-da390d4dfdf4" />

- (Explain the communication between them & include a block diagram )
### 🚀 RESTful API Usage
-Representational
-State
-Transfer
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
