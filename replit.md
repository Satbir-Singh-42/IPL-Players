# Player Dashboard

## Overview
A cricket player dashboard application for managing player rosters. This is a static HTML/CSS/JavaScript application that displays player cards with images and allows users to mark players as sold or restore them back to the active roster.

## Recent Changes
- **October 22, 2025**: Successfully migrated project to Replit environment
  - Installed Python 3.11 for serving static files
  - Configured workflow to serve the application on port 5000
  - Added .gitignore for Python and Replit files
  - Verified application is working correctly
  - **Added confetti animation effect** when marking players as sold
    - Integrated canvas-confetti library via CDN
    - Created multi-burst confetti animation with colorful particles (150 center + 100 left + 100 right)
    - Fixed confetti to render properly in fullscreen viewer mode
    - Animation plays for 2 seconds before auto-advancing to next player
  - **Added "UNSOLD" stamp effect** when marking players as unsold
    - Displays animated red "UNSOLD" stamp overlay on player image
    - Stamp appears with scale and rotation animation
    - Shows for 2 seconds before automatically moving to next player
    - Responsive sizing (400px desktop, 250px tablet, 180px mobile)

## Project Structure
- `index.html` - Main application file containing all HTML, CSS, and JavaScript
- `full_pngs/` - Directory containing all player images (127 player cards)
- `.gitignore` - Git ignore configuration
- `.local/state/replit/agent/progress_tracker.md` - Migration progress tracker

## Features
- **Player Gallery**: Displays all active players in a grid layout
- **Search**: Real-time search functionality to filter players by name
- **Statistics Counter**: Always-visible corner display showing Active/Sold/Unsold counts
- **Player Viewer**: Click any player to view their full image
- **Mark as Sold**: Move players from active roster to sold section with confetti animation
- **Mark as Unsold**: Skip players with animated stamp effect
- **Quick Undo (R key)**: Instantly undo last sold/unsold action
- **Restore Players**: Move sold players back to active roster
- **State Persistence**: Uses localStorage to remember sold/active player states
- **Mobile Responsive**: Touch-friendly interface with swipe gestures
- **Lazy Loading**: Optimized image loading for better performance
- **Keyboard Navigation**: Arrow keys to navigate, R key to undo

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
