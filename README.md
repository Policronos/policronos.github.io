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
            border-
