# Vert Per Hour - Strava Elevation Tracker

A web app to analyze elevation gain per hour for your Strava trail running activities.

## Features

- View elevation gain per hour for all your runs
- Filter by activity type (road runs vs trail runs) and time range
- Click on any bar to see detailed climb/descent rates over time
- Interactive charts with 1-minute rolling windows

## Setup Instructions

### Step 1: Create GitHub Repository

1. Go to https://github.com/edwardmonrad
2. Click "New repository" (green button)
3. Repository name: `vert-per-hour-strava-plugin`
4. Make it **Public**
5. Click "Create repository"

### Step 2: Upload the File

1. In your new repository, click "uploading an existing file"
2. Upload the `index.html` file from this download
3. Click "Commit changes"

### Step 3: Enable GitHub Pages

1. Go to **Settings** → **Pages** (in your repository)
2. Under "Source", select **main** branch
3. Click **Save**
4. Wait a few minutes - your site will be live at:
   ```
   https://edwardmonrad.github.io/vert-per-hour-strava-plugin
   ```

### Step 4: Update Your Strava API App

1. Go to https://www.strava.com/settings/api
2. Find your existing API application (or create a new one if needed)
3. **Update these fields:**
   - **Authorization Callback Domain:** `edwardmonrad.github.io`
   - **Website:** `https://edwardmonrad.github.io/vert-per-hour-strava-plugin`
4. Click "Update"

### Step 5: Use the App

1. Visit https://edwardmonrad.github.io/vert-per-hour-strava-plugin
2. Enter your Strava Client ID and Client Secret
3. Click "Connect with Strava"
4. Authorize the app
5. You'll be redirected back and your data will load!

## For Others to Use

Anyone can use this app! They just need to:

1. Visit your GitHub Pages URL
2. Create their own Strava API app at https://www.strava.com/settings/api
   - Set Authorization Callback Domain to: `edwardmonrad.github.io`
3. Enter their own Client ID and Client Secret
4. Connect and analyze their data!

## Privacy

- All data processing happens in the browser
- No data is sent to any server except Strava's API
- Client credentials are stored only temporarily in session storage
- Each user connects to their own Strava account

## Technical Details

- Built with React (via CDN)
- Uses Chart.js for visualizations
- Strava API OAuth 2.0 authentication
- Fully client-side - no backend required
