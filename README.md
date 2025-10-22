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

- **S** - Mark player as Sold (when viewing)
- **U** - Mark player as Unsold (when viewing)
- **C** - Close player viewer
- **R** - Quick Undo (reverses last Sold or Unsold action)
- **Arrow Left** - Previous player (when viewing)
- **Arrow Right** - Next player (when viewing)
- **Escape** - Close player viewer (alternative to C)

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

## 📝 Feature Summary

| Feature            | Status | Keyboard Shortcut |
| ------------------ | ------ | ----------------- |
| Search Players     | ✅     | -                 |
| Fullscreen Viewer  | ✅     | C or Escape       |
| Sold with Confetti | ✅     | S                 |
| Unsold with Stamp  | ✅     | U                 |
| Statistics Counter | ✅     | -                 |
| Quick Undo         | ✅     | R                 |
| Navigation         | ✅     | ← →               |
| State Persistence  | ✅     | -                 |
| Mobile Responsive  | ✅     | -                 |
| Restore Players    | ✅     | -                 |

---

## 📄 License

This project is for personal/internal use for IPL auction management.

---

## 🙏 Credits

- **canvas-confetti** by Kiril Vatev
- Player images from IPL official sources
