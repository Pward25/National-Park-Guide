# Overview

The Yosemite National Park Guide is an interactive web application that helps visitors explore Yosemite's most iconic landmarks, waterfalls, viewpoints, and recreational areas. The map features 24 carefully selected locations throughout the park, each marked with color-coded pins that indicate the type of attraction. Users can click on any marker to view detailed information including elevation, difficulty level, descriptions, and visitor tips.

To use the software, simply open the HTML file in a web browser. The map will load centered on Yosemite Valley with a satellite basemap view. Navigate by clicking and dragging to pan, scrolling to zoom in/out, or using the zoom controls. Click any marker to open a popup window with detailed information about that location. The markers are color-coded by type: red for iconic landmarks (Half Dome, El Capitan), blue for waterfalls, orange for viewpoints, turquoise for lakes, green for sequoia groves, and more.

The data for this project was compiled from official National Park Service information, elevation data from USGS sources, and personal research about trail difficulties and visitor recommendations. All geographic coordinates were verified using multiple mapping services to ensure accuracy.

[Software Demo Video](http://youtube.link.goes.here)

# Development Environment

The development environment for this project was intentionally kept minimal to focus on the core mapping functionality:

**Tools Used:**
* VS Code
* Web browser (Chrome/Firefox) with developer tools for testing and debugging
* ArcGIS CDN for loading the mapping library (no local installation required)

**Programming Language and Libraries:**
* **HTML5** - Structure and layout of the web application
* **CSS3** - Styling, responsive design, and visual polish
* **JavaScript (ES5/ES6)** - Application logic and interactivity
* **ArcGIS JavaScript API (version 4.28)** - Core mapping functionality including:
  - Map and MapView modules for rendering the base map
  - GraphicsLayer for managing marker layers
  - Graphic and Point modules for creating location markers
  - SimpleMarkerSymbol for customizing marker appearance
  - PopupTemplate for creating interactive information windows

The ArcGIS API uses the AMD (Asynchronous Module Definition) pattern with the `require()` function to load modules dynamically. This approach keeps the initial page load fast and only loads the components needed for the application.

# Useful Websites

* [ArcGIS JavaScript API Documentation](https://developers.arcgis.com/javascript/latest/) - Comprehensive documentation for all API features
* [ArcGIS API Reference Guide](https://developers.arcgis.com/javascript/latest/api-reference/) - Detailed reference for classes and methods
* [ArcGIS Tutorials](https://developers.arcgis.com/javascript/latest/tutorials/) - Step-by-step guides for common mapping tasks
* [National Park Service - Yosemite](https://www.nps.gov/yose/index.htm) - Official park information and data
* [MDN Web Docs](https://developer.mozilla.org/) - JavaScript, HTML, and CSS reference
* [USGS Elevation Data](https://www.usgs.gov/) - Verified elevation information for landmarks

# Future Work


* Implement a search feature to quickly locate specific landmarks
* Add photo galleries for each location using the National Park Service API
* Include seasonal information to help visitors plan trips based on time of year
* Implement user reviews and ratings for each location