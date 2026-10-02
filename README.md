<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>My Grid Layout</title>
    <style>
        body {
            background-color: #f4f4f4;
            font-family: Arial, sans-serif;
        }
        /* Purple glow title */
        h1 {
            font-size: 48pt;
            color: #000000;
            text-align: center;
            text-shadow:
                0 0 6px #E033FF,
                0 0 12px #E033FF,
                0 0 24px #E033FF;
            margin-bottom: 20px;
            line-height: 0.8;
            font-family: Constantia, "Lucida Bright", "DejaVu Serif", Georgia, serif;
        }
        /* FIXED GRID — no gaps */
        .photo-grid {
            display: grid;
            grid-template-columns: repeat(2, 384px);
            grid-auto-rows: 384px;
            gap: 10px;
            width: max-content;
            margin: 0 auto;
        }
        .photo-grid img {
            width: 384px;
            height: 384px;
            object-fit: cover;
        }
        .photo-grid img:nth-child(1) { grid-area: 1 / 1; }
        .photo-grid img:nth-child(2) { grid-area: 1 / 2; }
        .photo-grid img:nth-child(3) { grid-area: 2 / 1; }
        .photo-grid img:nth-child(4) { grid-area: 2 / 2; }
    </style>
</head>

<body>

<h1>My Grid Layout</h1>

<div class="photo-grid">
    <img src="IMG_4718.jpeg" alt="Photo 1">
    <img src="IMG_4719.jpeg" alt="Photo 2">
    <img src="IMG_4720.jpeg" alt="Photo 3">
    <img src="IMG_4716.jpeg" alt="Photo 4">
</div>

</body>
</html>
