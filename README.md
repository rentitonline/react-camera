# React Camera

A flexible camera component for React DOM; take photos using the latest WebRTC API's.

## Installation

React Camera is designed to be installed through NPM and imported as an ES6 module.

```
npm install react-dom-camera
```

Then import it into your project.

```javascript
import Camera from 'react-dom-camera';
```

## Usage

Here is a basic example of how to use React Camera in a React app. This will simply render the Camera component out of the box.

```javascript
import React from 'react';
import Camera from 'react-dom-camera';

const App = () => <Camera />;
```

### Taking a photo 📸

React Camera is setup to take an image of the current frame when the capture button is clicked, however to access the image you must use the `onTakePhoto` function which gives you the image.

```javascript
import React from 'react';
import Camera from 'react-dom-camera';

const App = () => (
  <Camera
    onTakePhoto={image =>
      console.log(image, 'do whatever you want with the image')
    }
  />
);
```
