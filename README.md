Landing Page Project

This repository contains the source code for a responsive landing page built with HTML, SCSS (Sass) and deployed on Vercel.

Live Demo
A live version of the project is available at:
https://landing-pi-silk.vercel.app

Features

Fully responsive layout
SCSS-based styling with modular structure
Background images and icons loaded from static assets
Easy-to-maintain folder structure
Fast build using Sass CLI

Technologies

HTML5
CSS3 (compiled from SCSS)
Sass (dart-sass)
Vercel (for deployment)

Installation

Clone the repository:
git clone https://github.com/Tima51-end/landing.git
cd landing

Install dependencies:
npm install

Development

To start working locally with live rebuilding of SCSS files:
npm run start
This will watch your SCSS files in src/scss/ and compile them to src/styles/styles.css on change.

Build

Before deploying or previewing a production build, run:
npm run build
This command compiles all SCSS into a single CSS file without source maps, ready for production.

Deployment to Vercel

Make sure your project is connected to a GitHub repository in your Vercel dashboard.
In Vercel settings, set the Build Command to:
npm run build
Leave the Output Directory empty (default is the project root).
Push your changes to GitHub. Vercel will automatically build and deploy your landing page.

Folder Structure

landing/
├─ node_modules/          # npm packages
├─ src/
│  ├─ scss/               # SCSS source files
│  │  ├─ _variables.scss  # Global variables
│  │  └─ main.scss        # Main stylesheet
│  ├─ styles/             # Compiled CSS
│  │  └─ styles.css
│  ├─ images/             # Background and content images
│  ├─ icons/              # SVG and icon assets
│  └─ index.html          # Main HTML file
├─ package.json           # Project metadata and scripts
├─ package-lock.json
└─ vercel.json            # Vercel rewrite rules and configuration

License

This project is released under the ISC License. See LICENSE for details.

