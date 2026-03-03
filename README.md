# Electrochem Viewer

A lightweight, purely browser-based web application for viewing, overlaying, and analyzing electrochemical measurements from Gamry Instruments.

This tool aims to provide a fast and interactive visualization of your electrochemical data without requiring any software installation or external servers.

## Features

- **Gamry Data Support**: Directly parses Gamry `.DTA` data files.
- **Data Overlay**: Easily select multiple files to overlay their graphs for direct comparison.
- **Dynamic Adjustments**: Built with Plotly.js to provide interactive plotting features including panning, zooming, and dynamic axis scaling.
- **CV & EIS Support**: Currently supports standard electrochemical formats:
  - **CV (Cyclic Voltammetry)**: Plots Current (µA) vs. Potential (V).
  - **EIS (Electrochemical Impedance Spectroscopy)**: Plots Nyquist (-Z'' vs Z') graphs with equal axis scaling.
- **Export Capabilities**: Easily export the interactive plots as vector graphics (SVG).

## How to Use

Since this is a client-side only web app, there's no installation or server setup required.

1. **Open the App**: Simply open `index.html` in any modern web browser (Chrome, Firefox, Edge, Safari).
2. **Import Data**: Click the **Import Data Folder** button on the sidebar.
3. **Select Folder**: Choose a local folder on your computer that contains your Gamry `.DTA` files. *Note: You must allow your browser permission to view the folder's files.*
4. **Select Files to Plot**: Check the boxes next to the filenames in the sidebar you wish to visualize. The app will automatically determine if the data is CV or EIS and plot it accordingly.
5. **Interact**: Use your mouse to click and drag to pan around the graph or use your scroll wheel to zoom in and out. 

## Technical Details

- **Zero Dependencies**: Simply built with standard HTML/CSS/JavaScript.
- **Library**: Utilizes the robust [Plotly.js](https://plotly.com/javascript/) library for performant and interactive data visualization.
- **Local Parsing**: The app securely parses all data structures locally within your browser. Thus, no experiment data is ever uploaded or sent over the internet.
