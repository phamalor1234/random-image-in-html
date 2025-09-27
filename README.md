# random-image-in-html

This repository demonstrates how to display a random image in HTML using JavaScript.

## Usage

1. Add your image files to an `images/` folder in your project directory.
2. Use the provided sample code below to display a random image on your webpage.

## Example

```html
<!DOCTYPE html>
<html>
<head>
  <title>Random Image Example</title>
</head>
<body>
  <img id="random-image" src="" alt="Random Image" width="300">
  <script>
    // Array of image paths
    const images = [
      'images/pic1.jpg',
      'images/pic2.jpg',
      'images/pic3.jpg',
      // Add more images as needed
    ];

    // Choose a random image
    const randomIndex = Math.floor(Math.random() * images.length);
    const selectedImage = images[randomIndex];

    // Set the src attribute of the image
    document.getElementById('random-image').src = selectedImage;
  </script>
</body>
</html>
```

## How it works

- The JavaScript script randomly selects an image from the array of image paths.
- The selected image will be displayed each time the page is loaded or refreshed.

## License

This project is open source and available under the MIT License.
