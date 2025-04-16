# animated-button<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<style>
    body {
        background-color: black;
        min-height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;



    }

    button {
        padding: 1em 2em;
        background-color: rgb(34, 34, 34);
        border: none;
        color: lightgray;
        border-radius: 1000px;
        font-size: 20px;
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        position: relative;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    button::after {
        content: '';
        position: absolute;
        height: 107%;
        width: 102%;
        border-radius: 100px;
        background-image: linear-gradient(to bottom right, rgb(10, 10, 243), rgb(255, 26, 255), red, rgb(137, 127, 249), rgb(0, 183, 255));
        z-index: -1;
    }

    button:hover {
        z-index: 0;
        box-shadow: 40px 0 100px rgb(10, 10, 243),
            -40px 0 100px red, -30px 0 100px rgb(255, 26, 255), -40px 0 100px rgb(47, 1, 255);
        opacity: 0.75;
    }
</style>

<body>
    <button>Gradient Button
    </button>
</body>

</html>
