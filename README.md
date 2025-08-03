# 🚁 Hoher Fläming Helicopter Explorer

An interactive web-based exploration game where you pilot a helicopter to discover 16 points of interest across the Hoher Fläming Nature Park in Brandenburg, Germany.

![Game Status](https://img.shields.io/badge/status-active-success)
![Version](https://img.shields.io/badge/version-2.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)

## 🎮 Game Overview

Explore the beautiful Hoher Fläming region from above! Your mission is to visit all 16 historical sites, castles, nature reserves, and viewpoints scattered across the map. Each location has its own unique story and significance to the region.

### Features

- **Realistic Flight Physics**: Smooth helicopter controls with momentum and drag
- **16 Unique Locations**: Discover castles, nature reserves, historic towns, and scenic viewpoints
- **Interactive Map**: Based on the actual Hoher Fläming Nature Park
- **Progress Tracking**: Visual indicators show which POIs you've visited
- **Multiple Control Options**: Keyboard, touch, and mouse support
- **Audio Feedback**: Dynamic engine sounds (optional)
- **Responsive Design**: Works on desktop, tablet, and mobile devices

## 🕹️ How to Play

### Controls

#### Desktop (Keyboard)
- **Arrow Keys** or **WASD**: Control helicopter movement
  - Up/W: Accelerate forward
  - Down/S: Slow down
  - Left/A: Turn left
  - Right/D: Turn right
- **L**: Land at nearby POI (when indicator appears)

#### Mobile/Tablet (Touch)
- **On-screen Joystick**: Drag to control direction and speed
- **Land Button**: Tap when near a POI to land and explore

#### Desktop (Mouse)
- **Click and drag** on the joystick for precise control

### Gameplay

1. **Start Location**: You begin at Bad Belzig (POI #7), home to the historic Burg Eisenhardt
2. **Navigation**: Fly your helicopter using the controls to explore the map
3. **Finding POIs**: Look for numbered yellow markers on the map
4. **Landing**: When you're near a POI (marker glows brighter), press L or tap the Land button
5. **Discovery**: Read about each location's history and significance
6. **Completion**: Visit all 16 POIs to complete your exploration mission

### Visual Indicators

- **Yellow Markers**: Unvisited POIs
- **Green Markers**: Visited POIs
- **Glowing Marker**: You're within landing range
- **HUD Display**: Shows current speed and progress (visited/total POIs)

## 📍 Points of Interest

1. **Stadt und Burg Ziesar** - Historic bishop's residence
2. **Gutspark Dahlen** - English-style park with historic vistas
3. **Klein Briesener Bach** - Protected stream area
4. **Paradies Dippmannsdorf** - Nature reserve with 30+ springs
5. **Töpferort Görzke** - Traditional pottery village
6. **Hagelberg** - Site of 1813 Napoleonic battle
7. **Bad Belzig mit Burg Eisenhardt** - Castle with panoramic views
8. **Aussichtspunkt Belziger Landschaftswiesen** - Bird sanctuary viewpoint
9. **Wiesenburg mit Schloss und Park** - Picturesque castle and park
10. **Naturparkzentrum Hoher Fläming** - Nature park information center
11. **Raben mit Burg Rabenstein** - Important border castle
12. **Niemegk** - Historic town with local culture
13. **Flämingbuchen** - Unique beech tree islands
14. **Brautrummel mit Riesenstein** - Periglacial valley with giant stone
15. **Neuendorfer Rummel** - Ice Age dry valley
16. **Garrey mit Aussichtsplattform** - Observation deck at old waterworks

## 🛠️ Technical Details

### Requirements
- Modern web browser (Chrome, Firefox, Safari, Edge)
- JavaScript enabled
- Internet connection (for loading map image)

### Technologies Used
- HTML5 Canvas
- CSS3 with animations
- Vanilla JavaScript
- Tone.js for audio synthesis
- No external dependencies required

### Browser Compatibility
- ✅ Chrome/Chromium (v90+)
- ✅ Firefox (v88+)
- ✅ Safari (v14+)
- ✅ Edge (v90+)
- ✅ Mobile Safari (iOS 14+)
- ✅ Chrome Mobile (Android)

## 🚀 Installation

### Quick Start
1. Download the HTML file
2. Open in a web browser
3. Start exploring!

### Hosting Online
```bash
# Clone or download the file
# Upload to any static web host
# No build process required!
```

### Local Development
```bash
# Option 1: Direct file opening
# Simply open the HTML file in your browser

# Option 2: Local server (recommended)
python -m http.server 8000
# or
npx http-server
```

## 🎯 Tips & Strategies

1. **Start Exploring Nearby**: Begin with POIs close to Bad Belzig
2. **Use the POI List**: Click the menu (☰) to see all locations
3. **Plan Your Route**: Check the map to create an efficient path
4. **Smooth Landing**: Reduce speed when approaching POIs for easier landing
5. **Mobile Play**: Use landscape orientation for better visibility

## 🐛 Troubleshooting

### Map Won't Load
- Check your internet connection
- Refresh the page
- Try a different browser
- Disable ad blockers temporarily

### Controls Not Working
- Ensure JavaScript is enabled
- Try refreshing the page
- Check if another application is capturing input

### Performance Issues
- Close other browser tabs
- Try a different browser
- Reduce browser zoom level
- Disable browser extensions

## 📱 Mobile Optimization

The game is fully optimized for mobile devices:
- Touch-friendly controls
- Responsive design adapts to screen size
- Landscape mode recommended
- Minimal battery usage
- Works offline after initial load

## 🎨 Customization

You can easily customize the game by modifying:
- Starting position (change `START_X` and `START_Y`)
- Flight physics (adjust `MAX_SPEED`, `ACCELERATION`, `DRAG`)
- Visual theme (modify CSS variables)
- POI data (add or modify locations)

## 📄 License

This game is open source and available under the MIT License. Feel free to modify and share!

## 🙏 Credits

- Map data: Hoher Fläming Nature Park
- Game design and development: Community contribution
- Audio library: Tone.js
- Helicopter emoji: System default

## 🔮 Future Enhancements

Potential features for future versions:
- [ ] Missions and challenges
- [ ] Time-based scoring
- [ ] Weather effects
- [ ] Fuel management
- [ ] Multiplayer exploration
- [ ] Additional regions to explore
- [ ] Achievement system
- [ ] Photo mode

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests
- Share your exploration experiences

---

**Happy Flying! 🚁**

*Explore the beauty and history of Hoher Fläming from above!*