# GeoEarn

GeoEarn is a tool I built to answer a practical question for freelancers: if you move to another city, what hourly rate would let you keep the same standard of living and savings?

I presented the project at NPS International School's 2nd AI & Robotics Symposium. It received **Best Technical Execution and Functionality** in the Senior Category on 19 August 2026.

## What it does

Enter your income, current hourly rate, home city, destination, and savings target. GeoEarn estimates the rate you would need in the destination and shows the cost assumptions behind it. You can compare 32 cities, inspect a basket of 70 everyday prices, view the route on a map, and save or export scenarios.

The advisor answers common questions about the current comparison using rules built into the page. It does not call an AI model or send your questions to a server.

## Running the project

Open [`index.html`](index.html) in a browser. Choose guest mode or create a profile that is stored on your device. There is no build step or backend. The page loads its fonts, styles, chart and map libraries, and map tiles from external CDNs, so those parts need an internet connection.

For GitHub Pages, go to **Settings > Pages**, select **Deploy from a branch**, and choose `main` and `/ (root)`.

## About the data

The city indices and price estimates are illustrative. I used public cost-of-living and purchasing-power references to calibrate the model; the links are on the Mission tab. Currency rates, taxes, visa information, and prices are embedded in the file and do not update automatically. This is a comparison tool, not financial, tax, or immigration advice.

Profiles and saved scenarios stay in your browser's local storage. They do not sync across devices, and clearing browser data removes them. The local password feature is intended to separate profiles on one device, not to protect sensitive information on a shared computer.

## Built with

HTML, CSS, and JavaScript in a single file, plus Tailwind CSS, Chart.js, Leaflet, Font Awesome, and Google Fonts. The map uses CARTO tiles and OpenStreetMap attribution.

This project has no open-source license at present. Please contact me before reusing the code.
