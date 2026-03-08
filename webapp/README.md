# Docker & Kubernetes Demo - Localhost Version

A simple, interactive webpage for teaching Docker and Kubernetes deployment concepts.

## Features

- Simple HTML page displaying "Hello Laxmi"
- Interactive button that shows a message on click
- Clean, modern UI with gradient background
- Easy to understand code structure for beginners

## Running Locally

### Using Python (Recommended)

```bash
cd webapp
python server.py
```

Then open your browser and navigate to: **http://localhost:8000**

### Using Node.js (Alternative)

```bash
cd webapp
npx http-server
```

Then open: **http://localhost:8080**

### Using Live Server in VS Code

1. Install the "Live Server" extension in VS Code
2. Right-click on `index.html` and select "Open with Live Server"

## Files Structure

- `index.html` - Main HTML file with page structure
- `style.css` - Styling for the webpage
- `script.js` - Interactive button functionality
- `server.py` - Simple Python HTTP server

## What It Does

1. Displays "Hello Laxmi" as the main heading
2. Has a blue button labeled "Click Me!"
3. When clicked, the button reveals: "Welcome to Docker And Kubernetes session"
4. Clean, responsive design that works on all screen sizes

## Next Steps

Once this works locally, we can:
- Containerize it with Docker
- Deploy it with Docker Compose
- Deploy it to Kubernetes with YAML manifests

---

**Created for educational purposes - Teaching Docker & Kubernetes basics**
