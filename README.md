# GeoLocation Data Pipeline & Visualization

## Overview
This project is a Python-based data pipeline that processes a list of global university locations, retrieves geolocation data from a web API, stores it in a structured SQLite database, and visualizes the results on an interactive map.

---

## Project Objective
To design an end-to-end data workflow that demonstrates data ingestion, API integration, data storage, and visualization using real-world location data.

---

## Situation
The dataset contained only university names without any geographic coordinates. This made it impossible to visualize or analyze their global distribution.

---

## Task
- Convert raw location names into geographic coordinates (latitude & longitude)
- Automate API data retrieval for multiple locations
- Store structured geolocation data efficiently
- Visualize all locations on a map

---

## Action

### 1. Data Ingestion
- Read location data from `where.data`
- Process each university name as a query input

### 2. API Integration
- Used a geocoding API (`opengeo`) to fetch location data
- Handled HTTP requests using `urllib`
- Parsed JSON responses using Python

### 3. Data Storage
- Designed SQLite database (`opengeo.sqlite`)
- Stored raw JSON responses for flexibility
- Implemented caching to avoid duplicate API calls

### 4. Data Processing
- Extracted latitude and longitude from JSON
- Handled missing or invalid responses
- Added rate limiting for API calls

### 5. Visualization
- Generated JavaScript file (`where.js`)
- Plotted locations on an interactive map
- Enabled visualization of all universities globally

---

## Result
- Successfully processed 100+ global university locations
- Built a reusable geolocation data pipeline
- Reduced redundant API calls through database caching
- Created a visual map representation of all locations
- Demonstrated end-to-end data engineering workflow

---

## Technologies Used

- **Programming:** Python
- **Data Handling:** JSON
- **Database:** SQLite
- **API Integration:** REST API (Geocoding)
- **Visualization:** JavaScript (Map-based plotting)
- **Libraries:** urllib, sqlite3, json, ssl

---
```
## Project Structure
├── geoload.py # Fetches geolocation data from API
├── geodump.py # Extracts data and prepares visualization
├── where.data # Input file (location names)
├── opengeo.sqlite # SQLite database storing API responses
├── where.js # JavaScript file for map visualization
├── where.html # Map visualization UI
├── README.md # Project documentation
```

---

## Key Learnings

- API integration and data retrieval
- JSON parsing and data transformation
- Database design and optimization
- Building data pipelines
- Geospatial data visualization
- Handling real-world data inconsistencies

---

## Future Improvements

- Add error logging and retry mechanisms
- Use advanced mapping tools (Google Maps / Leaflet)
- Store structured latitude/longitude separately
- Build a web dashboard for visualization
- Integrate cloud storage (AWS/GCP)

---

## Conclusion

This project demonstrates a complete data pipeline workflow — from raw input data to actionable visual insights — making it highly relevant for Data Engineer, Data Analyst, and Data Scientist roles.

---

## Images

<img width="665" height="945" alt="API Result in JSON" src="https://github.com/user-attachments/assets/0089d042-765f-4af9-8d21-2b9c4ad51ef6" />

---
