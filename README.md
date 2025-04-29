# Interactive Map - Hoher Fläming Region

## Description

This project is an interactive web map focused on the "Hoher Fläming" region in Brandenburg, Germany. It allows users to explore the area, view walking and cycling routes, find accommodation and local amenities, and filter the displayed information based on various criteria. It also includes a placeholder for real-time weather information.

The map interface is inspired by typical online map portals and aims to provide a user-friendly experience for planning trips and discovering points of interest in the region.

## Features

* **Interactive Base Map:**
    * Uses Leaflet.js for map rendering.
    * Includes OpenStreetMap as the default base layer.
    * Layer control allows switching between "Karte" (Map) and "Satellit" (Satellite) views.
    * Standard map controls (zoom in/out, panning).
* **Toggleable Data Layers:**
    * **Walking Routes:** Displays walking trails (placeholder data). Clicking highlights the route and shows details (name, length, duration, difficulty, tags) in a popup.
    * **Cycling Routes:** Displays cycling paths (placeholder data), similar interactivity to walking routes.
    * **Accommodation:** Shows markers for hotels, pensions, campsites, etc. (placeholder data). Clicking shows details. Uses Font Awesome icons.
    * **Local Amenities:** Displays markers for restaurants, stations, viewpoints, castles, churches, shops, etc. (placeholder data). Clicking shows details. Uses Font Awesome icons.
* **Interactive Sidebar:**
    * **Filtering:** Allows users to filter routes by:
        * Type (Walking/Cycling)
        * Difficulty (Easy/Medium/Hard)
        * Maximum Length (km)
        * Maximum Duration (h)
        * Starting Point / Named Route
        * Various Criteria (Public Transport Accessible, Family-Friendly, Stroller-Friendly, Wheelchair Accessible, Nordic Walking, Circular, Castle, Pottery, Church, Art, Hiking Trail) via checkboxes.
    * **POI Visibility:** Checkboxes to toggle the visibility of Accommodation and Amenity layers.
    * **Search:** A general search bar to find routes or points of interest by name or type.
    * **Controls:** "Apply Filters" and "Reset" buttons.
* **Weather Widget (Placeholder):**
    * A dedicated section in the sidebar to display current weather conditions for the Hoher Fläming region.
    * **Note:** Requires a valid API key from a weather service (like OpenWeatherMap) to fetch live data. See the `fetchWeather` function in the JavaScript code.
* **User Experience:**
    * Responsive design adapting to different screen sizes (desktop, tablet, mobile).
    * Sidebar toggles for mobile view.
    * Loading indicator during data filtering.
    * Clear visual distinction between route types and POI markers using colors and icons.
    * Route highlighting on click.

## Technology Stack

* **HTML:** Structure of the web page.
* **CSS:** Styling and layout.
    * **Tailwind CSS:** Utility-first framework for rapid UI development and responsiveness.
    * **Font Awesome:** For POI icons.
* **JavaScript:**
    * **Leaflet.js:** Core library for interactive maps.
    * Handles user interactions, filtering logic, data processing (currently placeholders), and UI updates.
    * Includes structure for `fetch` API calls (for loading real data and weather).

## Data

* **Current State:** The map currently uses **placeholder GeoJSON data** embedded directly in the JavaScript (`placeholderRoutes`, `placeholderPOIs`). This includes sample routes and points of interest based on the provided PDF documents.
* **Route Geometry:** The line geometries for routes are **placeholders** and do not represent the actual paths.
* **POI Coordinates:** Point of Interest coordinates are **approximations** based on town names or descriptions from the source documents, except for a few key locations where specific coordinates were provided.
* **Real Data:** For full functionality and accuracy, the placeholder data needs to be replaced with actual **GeoJSON or GPX files** for the Hoher Fläming region. The code includes commented-out `fetch` examples in the `loadInitialData` function showing where to load these external files.

## Setup & Usage

1.  Save the code as an HTML file (e.g., `hoher_flaeming_map.html`).
2.  Open the HTML file in a modern web browser (like Chrome, Firefox, Edge, Safari).
3.  The map interface will load with the placeholder data. Interact with the map controls and the sidebar filters.

## Weather API Integration

* To enable the live weather feature:
    1.  Sign up for a free API key from a weather service like [OpenWeatherMap](https://openweathermap.org/).
    2.  Locate the `fetchWeather` function in the JavaScript section of the HTML file.
    3.  Replace the placeholder string `'YOUR_OPENWEATHERMAP_API_KEY'` with your actual API key.
    4.  (Optional) Adjust the `lat` and `lon` variables if you want the weather for a different specific point within the region.

## Future Enhancements

* Load actual route data (GPX or GeoJSON) for accurate path display.
* Load actual POI data with precise coordinates.
* Refine and expand the POI icons using Leaflet plugins or custom SVGs.
* Implement more sophisticated search functionality (e.g., searching within descriptions).
* Add dynamic population of filter dropdowns (e.g., Start Points) based on loaded data.
* Improve error handling for data loading and API calls.
* Add functionality to display route elevation profiles (requires elevation data).

