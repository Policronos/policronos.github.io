<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Sliders</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 50px;
            background-color: #f4f4f9;
        }
        .slider-container {
            margin-bottom: 25px;
            max-width: 300px;
        }
        label {
            font-weight: bold;
            display: block;
            margin-bottom: 5px;
        }
        input[type="range"] {
            width: 100%;
        }
        .value-display {
            color: #555;
            font-size: 0.9em;
        }
    </style>
</head>
<body>

    <h2>Interactive Sliders</h2>

    <div class="slider-container">
        <label for="slider1">Slider A</label>
        <input type="range" id="slider1" min="0" max="100" value="50" oninput="updateValue('slider1', 'val1')">
        <div class="value-display">Value: <span id="val1">50</span></div>
    </div>

    <div class="slider-container">
        <label for="slider2">Slider B</label>
        <input type="range" id="slider2" min="0" max="100" value="50" oninput="updateValue('slider2', 'val2')">
        <div class="value-display">Value: <span id="val2">50</span></div>
    </div>

    <div class="slider-container">
        <label for="slider3">Slider C</label>
        <input type="range" id="slider3" min="0" max="100" value="50" oninput="updateValue('slider3', 'val3')">
        <div class="value-display">Value: <span id="val3">50</span></div>
    </div>

    <script>
        // Function to update the displayed text dynamically
        function updateValue(sliderId, displayId) {
            const sliderValue = document.getElementById(sliderId).value;
            document.getElementById(displayId).textContent = sliderValue;
        }
    </script>

</body>
</html>
