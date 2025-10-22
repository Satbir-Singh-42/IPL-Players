# 🏏 Player Dashboard - IPL Auction Manager

A modern, feature-rich cricket player dashboard application designed for managing IPL auction workflows. Built with pure HTML, CSS, and JavaScript for lightning-fast performance.

---

## ✨ Features

### 🎴 Player Management
- **127 Player Cards** - Complete roster with high-quality player images
- **Search Functionality** - Real-time search to filter players by name
- **Lazy Loading** - Optimized image loading for better performance
- **Hover Preloading** - Images load on hover for instant viewing

### 📊 Statistics Counter
- **Real-time Stats** - Always visible counter showing:
  - Active Players
  - Sold Players
  - Unsold Players
- **Corner Display** - Small, non-intrusive counter in top-right corner
- **Works in Fullscreen** - Stats remain visible even when viewing players in fullscreen mode

### 🎯 Auction Actions

#### Sold Button
- **Confetti Animation** - Celebratory confetti burst with 3 waves:
  - 150 particles from center
  - 100 particles from left
  - 100 particles from right
- **Auto-move** - Automatically moves to next player after 1 second
- **State Persistence** - Sold players saved to separate section
- **Restore Option** - Sold players can be restored back to active roster

#### Unsold Button
- **Stamp Effect** - Animated "UNSOLD" stamp overlay appears on player image
- **Scale Animation** - Stamp scales up with slight rotation
- **Auto-move** - Automatically moves to next player after 1 second
- **Counter Update** - Unsold count updates in real-time

### ⌨️ Keyboard Shortcuts
- **R** - Quick Undo (reverses last Sold or Unsold action)
- **Arrow Left** - Previous player (when viewing)
- **Arrow Right** - Next player (when viewing)
- **Escape** - Close player viewer

### 🔄 Quick Undo (R Key)
- Instantly undo the last action
- Works for both Sold and Unsold actions
- Press "R" anytime to reverse your last decision
- Restores player to active roster (for sold actions)
- Decrements unsold counter (for unsold actions)

### 🎨 Visual Effects
- **Fullscreen Viewer** - Click any player card to view in fullscreen
- **Smooth Animations** - Polished transitions and effects
- **Dark Theme** - Eye-friendly dark color scheme
- **Responsive Design** - Works on desktop, tablet, and mobile devices

### 💾 Data Persistence
- **localStorage** - All actions saved automatically
- **State Recovery** - Resume exactly where you left off
- **Reset Option** - "Reset View" button to start fresh

### 📱 Mobile Optimization
- **Touch Gestures** - Swipe left/right to navigate between players
- **Responsive Sizing** - Stamp and buttons adapt to screen size
- **Touch-friendly** - All buttons meet minimum touch target size (44px)

---

## 🚀 How to Use

### Starting the Auction
1. Open the application
2. Click on any player card to begin
3. Player opens in fullscreen viewer

### Managing Players
**Mark as Sold:**
- Click green "Sold" button
- Enjoy the confetti celebration 🎊
- Player moves to "Sold Players" section
- Auto-advances to next player in 1 second

**Mark as Unsold:**
- Click red "Unsold" button
- See the "UNSOLD" stamp effect 🏷️
- Counter updates
- Auto-advances to next player in 1 second

**Quick Undo:**
- Press "R" key anytime to undo last action
- Works for both sold and unsold decisions

### Navigation
- **Arrow Keys** - Navigate between players when viewing
- **Escape** - Close viewer and return to gallery
- **Search Box** - Type player name to filter
- **Reset View** - Clear all sold/unsold data and start over

### Restoring Players
- Scroll to "Sold Players" section
- Click "Restore" button on any sold player
- Player returns to active gallery in numerical order

---

## 📊 Statistics Tracking

The stats counter shows:
- **Active** - Players still in the active roster (green)
- **Sold** - Players marked as sold (gold)
- **Unsold** - Players marked as unsold (red)

All statistics update in real-time and persist across sessions.

---

## 🎯 Workflow Tips

1. **Fast Auction Mode:**
   - Use keyboard shortcuts for speed
   - Let auto-advance handle navigation
   - Press "R" immediately if you make a mistake

2. **Search & Process:**
   - Search for specific players
   - Process them quickly
   - Clear search to return to full roster

3. **Review & Adjust:**
   - Check sold players section anytime
   - Use restore button to fix mistakes
   - Stats counter keeps you informed

---

## 🛠️ Technical Details

### Built With
- **HTML5** - Semantic markup
- **CSS3** - Modern styling and animations
- **JavaScript** - Vanilla JS, no frameworks
- **canvas-confetti** - Confetti animation library
- **Python HTTP Server** - Local development server

### Performance Features
- Intersection Observer API for lazy loading
- Image caching system
- Aggressive preloading (first 20 images)
- Hover preloading for adjacent images
- Throttled scroll events

### Browser Support
- Chrome/Edge (recommended)
- Firefox
- Safari
- Mobile browsers (iOS Safari, Chrome Mobile)

---

## 📁 Project Structure

```
.
├── index.html                          # Main application file
├── full_pngs/                          # Player images directory
│   ├── 1 Virat Kohli.png
│   ├── 2 Suryakumar Yadav.png
│   └── ... (127 players)
├── attached_assets/                    # UI assets
│   └── unsold_1761163848644.png       # Unsold stamp image
├── replit.md                           # Project documentation
└── README.md                           # This file
```

---

## 🎨 Design Features

- **Dark Theme** - `#0d1117` background with `#e6edf3` text
- **Card Hover Effects** - Smooth `translateY(-5px)` on hover
- **Rounded Corners** - Modern 16px border radius
- **Shadow Effects** - Subtle depth with `rgba(0,0,0,0.4)` shadows
- **Gradient Buttons** - Eye-catching button designs
- **Smooth Transitions** - 0.2-0.4s ease transitions throughout

---

## 🔧 Development

### Running Locally
The application runs on port 5000 using Python's HTTP server:
```bash
python -m http.server 5000
```

### Making Changes
1. Edit `index.html` for all changes (styles, scripts, markup)
2. Restart the server workflow
3. Hard refresh browser (Ctrl/Cmd + Shift + R)

---

## 📝 Feature Summary

| Feature | Status | Keyboard Shortcut |
|---------|--------|-------------------|
| Search Players | ✅ | - |
| Fullscreen Viewer | ✅ | Escape to close |
| Sold with Confetti | ✅ | - |
| Unsold with Stamp | ✅ | - |
| Statistics Counter | ✅ | - |
| Quick Undo | ✅ | R |
| Navigation | ✅ | ← → |
| State Persistence | ✅ | - |
| Mobile Responsive | ✅ | - |
| Restore Players | ✅ | - |

---

## 🎯 Version History

**v1.0.0** - October 22, 2025
- Initial release
- 127 player cards
- Sold/Unsold functionality
- Confetti and stamp effects
- Statistics counter
- Quick undo feature
- Keyboard shortcuts
- State persistence
- Mobile optimization

---

## 📄 License

This project is for personal/internal use for IPL auction management.

---

## 🙏 Credits

- **canvas-confetti** by Kiril Vatev
- Player images from IPL official sources
- Built with ❤️ for smooth auction experiences

---

**Enjoy your auction! 🏏🎉**
