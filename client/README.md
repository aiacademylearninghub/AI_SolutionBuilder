# Solution Builder Client
Solution Builder Client is responsible for handling the frontend operations and providing a user interface for the application. It interacts with the Solution Builder Server to fetch data and display it to the user.

## Setup
To setup the Solution Builder Client, follow these steps:
1. Navigate to the client directory
```cmd
cd client
```
2. Install dependencies
```cmd
npm install
```
3. Run the client
```cmd
npm start
```

## UI Features and Styling

The Solution Builder Client features a modern, attractive UI with the following enhancements:

- **Fully Responsive Design**: Optimized layouts for mobile, tablet, and desktop with fluid transitions
- **Smooth Animations**: Enhanced fade-in, slide, pulse, and float effects for a dynamic user experience
- **Theme Toggle**: Switch between light and dark modes with automatic UI adaptation
- **Glassmorphism Effects**: Modern frosted glass UI elements for depth and visual appeal
- **Card View**: Beautifully styled cards with hover effects, elevation changes, and accent borders
- **Tree View**: Enhanced tree navigation with interactive elements and scroll management
- **Floating Controls**: Easy access to application functions via an animated, responsive control panel
- **Gradient Color Scheme**: Professional gradient-based color scheme with primary (#4a6bdf) and secondary (#8076c8) colors
- **Interactive Elements**: Buttons and controls with hover effects, ripple animations, and visual feedback
- **Code Editor Integration**: Responsive and seamless integration with code sandbox when enabled

The UI implements modern design principles with attention to:
- Consistent spacing and typography across all device sizes
- Visual feedback for user interactions with smooth transitions
- Mobile-first responsive approach with breakpoint optimizations
- Accessible color contrast and keyboard navigation
- Custom scrollbars and performance optimizations
- Touch-friendly controls for mobile users

---

## Project File Documentation

### Client Folder (`client/`)

- **package.json**: Manages frontend dependencies, scripts, and project metadata for the React application.
- **public/**
  - **index.html**: The main HTML template for the React app.
  - **decision_tree.json**: Stores the decision tree data used for solution building.
  - **favicon.ico**, **robots.txt**: Standard web assets.
- **src/**
  - **index.js**: Entry point for the React app; sets up routing and renders the main component.
  - **constants.js**: Defines constants such as the backend server URL.
  - **components/**
    - **CardView.js**: React component for displaying questions, answers, and architecture diagrams in a card format.
    - **TreeView.js**: React component for rendering the decision tree structure visually.
  - **hooks/**
    - **useCodeSandbox.js**: Custom React hook to interact with the backend and CodeSandbox API for code template generation.
  - **pages/SolutionBuilder/**
    - **SolutionBuilder.js**: Main page component; manages state, fetches decision tree data, and coordinates UI layout.
    - **decisionTreeData.js**: Functions to build and process the decision tree structure from JSON data.
    - **mermaidText.js**: Functions to generate and update Mermaid diagram text for architecture visualization.
    - **SolutionBuilder.css**: Styles for the SolutionBuilder page.

---


This documentation provides a clear overview of each file's role, making it easier for LLMs and developers to understand and extend the Solution Builder application.
