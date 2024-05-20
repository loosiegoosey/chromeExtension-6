## Overview

Overview
This project is a simple Chrome extension that automatically detects the user's location when a button is pressed. If the location permissions are granted, the extension will replace the default location with the user's current geographical coordinates.

##
## Features

Features
- **Location Detection:** Automatically detects and uses the user's current location if permissions are granted.
- **Default Location:** Falls back to a predefined location (Codesmith Venice) if location access is not granted.

##
## Installation Instructions

Installation Instructions

1. **Clone the repository:**
   ```sh
   git clone https://github.com/iancdavis/chromeExtension.git
   ```
   
2. **Navigate to the project directory:**
   ```sh
   cd chromeExtension
   ```

3. **Load the extension in Chrome:**
   - Open Chrome and navigate to `chrome://extensions/`.
   - Ensure "Developer mode" is enabled.
   - Click "Load unpacked" and select the project directory.

##
## Usage Examples

Usage Examples
1. **Opening the Extension:**
   - Open Chrome and click on the extension icon in the toolbar.

2. **Using the Extension:**
   - Click the start button in the extension's popup.
   - If location access is granted, the user's current location will be obtained.
   - If location access is not granted, the default location will be used (Codesmith Venice).

```javascript
const startButton = document.querySelector('button');

startButton.addEventListener('click', () => {
    let userLat = 33.989060922556085;
    let userLong = -118.46904988298537;

    // Additional code to handle location detection
    // navigator.permissions.query({name:'geolocation'}).then(function(result) {
    //     if (result.state == 'granted') {
    //         obtainLocation(true);
    // }
});
```

##
## Code Summary

Code Summary
The project consists of a single JavaScript file that handles the main functionality of the Chrome extension.

- **index.js:**
  - Selects the start button using `document.querySelector`.
  - Adds an event listener to the start button to handle the click event.
  - If location access is granted, the user's location is obtained.
  - If location access is not granted, a default location (Codesmith Venice) is used.

##
## License

License
This project is licensed under the MIT License.

```
MIT License

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:
...

See the full license text in the LICENSE file.
```
```

Feel free to open issues or contribute to the project through pull requests!

```