# Colombia Travel Map - Specification

## Project Overview
- **Project name**: Colombia Travel Map
- **Type**: Interactive 3D globe/map webapp
- **Core functionality**: An interactive 3D globe centered on Colombia showing visited locations with timeline and statistics
- **Target users**: Anyone tracking travels within Colombia

## UI/UX Specification

### Layout Structure
- **Header**: Logo/title with minimal navigation
- **Hero**: Full-screen 3D interactive globe
- **Stats Panel**: Floating cards showing statistics (top-right)
- **Sidebar**: Left sidebar with location list and filters
- **Footer**: Minimal footer with credits

### Responsive Breakpoints
- Desktop: 1200px+
- Tablet: 768px - 1199px
- Mobile: < 768px

### Visual Design

#### Color Palette
- Background: `#0a0a0f` (deep dark blue-black)
- Primary: `#f9c74f` (golden yellow - Colombia flag)
- Secondary: `#f94144` (red - Colombia flag)
- Accent: `#43aa8b` (green - Colombia flag)
- Text Primary: `#ffffff`
- Text Secondary: `#94a3b8`
- Card Background: `rgba(15, 23, 42, 0.85)`
- Border: `rgba(148, 163, 184, 0.2)`

#### Typography
- Font Family: "Syne", sans-serif (headings), "DM Sans", sans-serif (body)
- Heading sizes: H1: 3rem, H2: 2rem, H3: 1.5rem
- Body: 1rem
- Small: 0.875rem

#### Spacing System
- Base unit: 8px
- Margins: 16px, 24px, 32px, 48px
- Padding: 12px, 16px, 24px
- Border radius: 8px (cards), 4px (buttons), 50% (avatars)

#### Visual Effects
- Glassmorphism cards with backdrop-filter blur
- Subtle glow effects on interactive elements
- Smooth transitions (0.3s ease)
- Hover scale effects on cards
- Animated markers on globe

### Components

1. **3D Globe**
   - Interactive globe using Three.js
   - Auto-rotation when idle
   - Click/drag to rotate
   - Zoom in/out
   - Colombia centered by default
   - Animated markers for visited locations
   - Atmosphere glow effect

2. **Stats Cards**
   - Total locations visited
   - Cities visited
   - Total trips
   - Latest location
   - Hover: slight lift + glow

3. **Location List**
   - Scrollable sidebar list
   - Each item shows: city name, date, thumbnail
   - Click to focus on globe
   - Hover effect

4. **Timeline**
   - Vertical timeline showing visit history
   - Date and location details
   - Connecting lines with dots

5. **Search/Filter**
   - Search input for locations
   - Filter by region/type

## Functionality Specification

### Core Features
1. Interactive 3D globe with Colombia centered
2. Clickable location markers
3. Auto-rotation animation
4. Statistics display
5. Location list with details
6. Timeline view of visits
7. Search functionality
8. Responsive design

### User Interactions
- Drag to rotate globe
- Scroll to zoom
- Click marker to see details
- Click location in list to focus
- Hover effects on all interactive elements

### Data Handling
- Static JSON data for locations
- No backend required
- Client-side rendering

### Sample Data (for demo)
- Bogotá (capital)
- Medellín
- Cartagena
- Cali
- Barranquilla
- Santa Marta
- Bucaramanga
- Pereira
- Manizales
- Armenia

## Acceptance Criteria
1. Page loads without errors
2. 3D globe renders and is interactive
3. At least 10 Colombian cities as markers
4. Stats display correctly
5. Location list is functional
6. Responsive on mobile/tablet
7. Smooth animations throughout
8. Visual design matches Colombia theme (yellow/red/green)
