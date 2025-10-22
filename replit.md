# Player Dashboard

## Overview
A cricket player dashboard application for managing player rosters. This is a static HTML/CSS/JavaScript application that displays player cards with images and allows users to mark players as sold or restore them back to the active roster.

## Recent Changes
- **October 22, 2025**: Successfully migrated project to Replit environment
  - Installed Python 3.11 for serving static files
  - Configured workflow to serve the application on port 5000
  - Added .gitignore for Python and Replit files
  - Verified application is working correctly

## Project Structure
- `index.html` - Main application file containing all HTML, CSS, and JavaScript
- `full_pngs/` - Directory containing all player images (127 player cards)
- `.gitignore` - Git ignore configuration
- `.local/state/replit/agent/progress_tracker.md` - Migration progress tracker

## Features
- **Player Gallery**: Displays all active players in a grid layout
- **Search**: Real-time search functionality to filter players by name
- **Player Viewer**: Click any player to view their full image
- **Mark as Sold**: Move players from active roster to sold section
- **Restore Players**: Move sold players back to active roster
- **State Persistence**: Uses localStorage to remember sold/active player states
- **Mobile Responsive**: Touch-friendly interface with swipe gestures
- **Lazy Loading**: Optimized image loading for better performance
- **Keyboard Navigation**: Arrow keys to navigate between players

## Technology Stack
- Pure HTML5, CSS3, and JavaScript (no frameworks)
- localStorage for data persistence
- Python HTTP server for serving static files
- Intersection Observer API for lazy loading
- Touch event handling for mobile devices

## Running the Application
The application is served using Python's built-in HTTP server on port 5000. The workflow is configured to automatically start the server when the Repl runs.

## User Preferences
None documented yet.

## Project Architecture
This is a single-page application with all code contained in `index.html`. The application uses:
- CSS Grid for responsive layout
- Intersection Observer for performance optimization
- Event delegation for dynamic content handling
- LocalStorage API for state management
