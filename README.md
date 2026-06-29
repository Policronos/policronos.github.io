<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Dark Sliders</title>
    <style>
        /* Dark theme setup and centering */
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #121214;
            color: #e2e8f0;
            margin: 0;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
        h2 {
            margin-bottom: 30px;
            color: #ffffff;
            letter-spacing: 0.5px;
        }
        /* Container for the sliders */
        .sliders-wrapper {
            width: 100%;
            max-width: 320px;
            padding: 20px;
            background-color: #1a1a1e;
            border-radius: 12px;
            box-shadow: 0 8px 24px rgba(0, 0, 0, 0.2);
        }
        .slider-container {
            margin-bottom: 25px;
        }
        .slider-container:last-child {
            margin-bottom: 0;
        }
        label {
            font-weight: 600;
            display: block;
            margin-bottom: 8px;
            color: #94a3b8;
            font-size: 0.9em;
        }
        /* Dark theme slider styling */
        input[type="range"] {
            width: 100%;
            accent-color: #3b82f6; /* Modern blue accent for the slider handle */
            background: #334155;
            height: 6px;
            border-radius: 5px;
            cursor: pointer;
        }
        .value-display {
            color: #3b82f6;
            font-size: 0.9em;
            margin-top: 6px;
            font-weight: bold;
            text-align: right;
        }
    </style>
</head>
<body>
    <h2>Interactive Sliders</h2>
    <div class="sliders-wrapper">
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
    </div>
    <script>
        function updateValue(sliderId, displayId) {
            const sliderValue = document.getElementById(sliderId).value;
            document.getElementById(displayId).textContent = sliderValue;
        }
    </script>
</body>
</html>
