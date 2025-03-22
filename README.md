<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flor Amarilla Animada</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #fff8dc;
        }
        svg {
            width: 200px;
            height: 300px;
        }
        .animate {
            stroke-dasharray: 300;
            stroke-dashoffset: 300;
            animation: grow 3s linear forwards;
        }
        @keyframes grow {
            to {
                stroke-dashoffset: 0;
            }
        }
    </style>
</head>
<body>
    <svg viewBox="0 0 200 300">
        <!-- Tallo -->
        <line x1="100" y1="250" x2="100" y2="100" stroke="green" stroke-width="4" class="animate"/>

        <!-- Hojas -->
        <path d="M100 170 C120 150, 140 160, 120 180" fill="green" stroke="green" stroke-width="2" class="animate"/>
        <path d="M100 190 C80 170, 60 180, 80 200" fill="green" stroke="green" stroke-width="2" class="animate"/>

        <!-- Pétalos -->
        <circle cx="100" cy="80" r="20" fill="yellow" class="animate"/>
        <circle cx="80" cy="90" r="20" fill="yellow" class="animate"/>
        <circle cx="120" cy="90" r="20" fill="yellow" class="animate"/>
        <circle cx="90" cy="70" r="20" fill="yellow" class="animate"/>
        <circle cx="110" cy="70" r="20" fill="yellow" class="animate"/>

        <!-- Centro de la flor -->
        <circle cx="100" cy="80" r="10" fill="brown" class="animate"/>
    </svg>
</body>
</html>
