# NASA APOD Portfolio Demo

This project demonstrates how to work with NASA's Astronomy Picture of the Day (APOD) API by simulating its functionality with local JSON data.  
It is part of a technical writing and development portfolio to showcase documentation skills, clear code samples, and interactive web output.

---

##  Project Overview
- Fetches and displays **random astronomy pictures** (simulated with JSON).  
- Written with **HTML, CSS, and JavaScript**.  
- Designed for **GitHub Pages hosting** (works without a backend).  
- Demonstrates **technical writing + API integration concepts**.  

Since GitHub Pages cannot securely store API keys, the project uses a **local JSON file (`apod-data.json`)** containing 20 sample astronomy entries with placeholder images and extended descriptions.
## Folder Structure

apod-portfolio/  
    - index.html # Main webpage  
    - style.css # Basic styling  
    - script.js # Handles random image selection  

data/  
    - apod-data.json # Sample APOD entries (20 total)

images/   # Placeholder astronomy images

## Setup Instructions

### 1. Clone the repository
```bash
git clone https://github.com/<your-username>/apod-portfolio.git
cd apod-portfolio

## Example Entry
```json
{
  "title": "Galaxy Cluster",
  "date": "2025-01-01",
  "explanation": "This galaxy cluster contains hundreds of galaxies bound together by gravity. The immense mass warps space-time, acting as a gravitational lens that magnifies background galaxies, helping astronomers study the distant universe.",
  "url": "images/Galaxy Cluster.jpg",
  "media_type": "image"
}

## Working with the Real NASA API

To use NASA's live APOD API:

1. Get a free API key: https://api.nasa.gov
2. Replace the local JSON fetch in `script.js` with:

```javascript
const response = await fetch("https://api.nasa.gov/planetary/apod?count=1&api_key=<YOUR_API_KEY>");
const data = await response.json();

## Portfolio Note

This project demonstrates:
- Technical documentation skills
- API integration walkthroughs
- Web development (HTML, CSS, JS)
- Simulation of live APIs for safe public hosting


