CLIMATE RESPONSE NETWORK — PROFESSIONAL PUNE PROTOTYPE
=======================================================

WHAT'S INCLUDED
- Responsive public dashboard with clean user-facing navigation.
- Live weather conditions and forecast from Open-Meteo (internet required).
- OpenStreetMap map tiles and nearby mapped health facility listings from Overpass API (internet required).
- Incident form with manually entered emergency type, optional browser geolocation and reverse geocoding.
- Local report history, demo staff sign-in, incident review status and CSV export.
- Official emergency call shortcut to 112.
- Response optimizer prototype: geocodes a typed incident area and ranks mapped health facilities by OSRM estimated road-route duration.

RUN ON WINDOWS / XAMPP
1. Extract the ZIP.
2. Copy the folder "climate_response_network" into C:\xampp\htdocs\
3. Start Apache in XAMPP Control Panel.
4. Open http://localhost/climate_response_network/
5. Staff demo login: open http://localhost/climate_response_network/admin.html
   Username: admin
   Password: PuneAdmin#2026

REAL DATA / IMPORTANT LIMITATIONS
- Weather is fetched live from Open-Meteo at Pune reference coordinates (18.5204, 73.8567). The simple "weather context" score is an illustrative calculation, NOT an official risk warning.
- Health facility locations come from community-maintained OpenStreetMap / Overpass data. Listings may be incomplete or stale. They do NOT show live bed/ICU availability, operating status, ambulance locations or verified emergency capacity.
- Browser geolocation and reverse geocoding require internet and user permission. On some browsers, location works only on localhost or HTTPS.
- Reports are stored in the current browser's localStorage. They are not sent to a server, hospital, police, ambulance, NDMA, IMD or ERSS.
- The staff login is a front-end demo credential and can be inspected in source code. It is NOT secure authentication. The staff console only reads local reports from the same browser profile.
- The response optimizer uses public geocoding and OSRM road-network estimates; these are not live traffic and do not include current road closures or disaster-damaged roads.
- No permission has been requested from government agencies because this prototype does not connect to their systems. Authorized ERSS/hospital/ambulance integration would require formal approval, documented APIs, security review and an agreed operating process.
- In a genuine urgent emergency in India, call 112. Do not rely on this student prototype to request rescue.

DATA / SERVICE LINKS
Open-Meteo: https://open-meteo.com/
OpenStreetMap: https://www.openstreetmap.org/copyright
Overpass API: https://overpass-api.de/
IMD official website: https://mausam.imd.gov.in/
ERSS 112: https://112.gov.in/

This is a student/hackathon prototype. Do not store sensitive or personally identifiable emergency information in it.

ROUTING / HUMANITARIAN DATA
OSRM demo: https://project-osrm.org/
HDX: https://data.humdata.org/
HOT on HDX: https://data.humdata.org/organization/hot

UI NOTES
The established green/mint visual theme has been retained and refined with responsive layouts, hover/focus states, map and form styling, and improved mobile navigation presentation.

ADDITIONAL HC-05 FEATURES
- Hazard watch panel mirrors the weather API values and links to official IMD advisories; it does not claim to receive official warnings.
- Resource planner calculates a simple units-needed estimate from user-entered affected people and planning capacity.
- Hospital capacity register allows manual local entries and explicitly labels them as unverified browser-only entries.
- Impact analytics summarizes browser-local incident reports by severity and type.
- Admin console supports searching and filtering incident records by severity and status.
- Smart route optimizer ranks mapped facility options by public OSRM estimated road time. It does not account for live traffic, road closures or flood-damaged roads.
