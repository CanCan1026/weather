# Weather Widget

## Overview

A simple, client-side weather widget designed to display scrolling weather information in a compact horizontal banner format. The widget features a modern gradient design with marquee-style text animation and appears to be built for embedding or use as a desktop widget component.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Pure HTML/CSS/JavaScript**: Single-page application using vanilla web technologies without any frameworks
- **Client-side rendering**: All functionality runs directly in the browser
- **Widget-based design**: Compact 60px height banner optimized for minimal screen real estate
- **Responsive layout**: Uses CSS flexbox and viewport-relative units for adaptability

### UI/UX Design Patterns
- **Marquee animation**: 30-second linear scrolling animation for continuous weather updates display
- **Configuration mode**: Expandable interface (minimum 200px height) for widget setup
- **Modern styling**: Uses system fonts and CSS gradients for clean, native appearance
- **Minimal footprint**: Designed to be unobtrusive with transparent background support

### Animation System
- **CSS-based animations**: Hardware-accelerated transforms for smooth scrolling
- **Continuous loop**: Infinite marquee effect for weather information display
- **Performance optimized**: Uses transform properties for better rendering performance

## External Dependencies

### Weather Data Source
- **Windy API Integration**: Uses Windy Point Forecast API v2 for weather data
- **Endpoint**: POST https://api.windy.com/api/point-forecast/v2
- **Authentication**: Requires Windy API key from api.windy.com
- **Data Model**: Uses GFS (Global Forecast System) weather model
- **Parameters**: Fetches temperature, wind, humidity, pressure, and precipitation data
- **Coordinate-based**: Requires latitude/longitude coordinates for each location
- **Real-time updates**: Displays current weather conditions with auto-refresh capability

### Browser Requirements
- **Modern CSS support**: Requires browsers with CSS Grid, Flexbox, and transform animation support
- **JavaScript enabled**: Client-side functionality dependent on browser JavaScript execution