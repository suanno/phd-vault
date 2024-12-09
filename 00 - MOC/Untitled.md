<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Clickable Triangular Cells</title>
    <style>
        table {
            border-collapse: collapse;
            margin: 20px;
        }
        td {
            position: relative;
            width: 100px;
            height: 100px;
            border: 1px solid #000;
        }
        .cell {
            position: absolute;
            width: 100%;
            height: 100%;
            clip-path: polygon(0 0, 100% 0, 0 100%);
        }
        .cell.top-left {
            background-color: lightblue;
        }
        .cell.bottom-right {
            background-color: lightcoral;
            clip-path: polygon(100% 0, 100% 100%, 0 100%);
        }
        .cell a {
            display: block;
            width: 100%;
            height: 100%;
            text-decoration: none;
        }
    </style>
</head>
<body>
    <table>
        <tr>
            <td>
                <div class="cell top-left">
                    <a href="#top-left" onclick="alert('Top Left Clicked!')"></a>
                </div>
                <div class="cell bottom-right">
                    <a href="#bottom-right" onclick="alert('Bottom Right Clicked!')"></a>
                </div>
            </td>
            <td>
                <div class="cell top-left">
                    <a href="#top-left" onclick="alert('Top Left Clicked!')"></a>
                </div>
                <div class="cell bottom-right">
                    <a href="#bottom-right" onclick="alert('Bottom Right Clicked!')"></a>
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div class="cell top-left">
                    <a href="#top-left" onclick="alert('Top Left Clicked!')"></a>
                </div>
                <div class="cell bottom-right">
                    <a href="#bottom-right" onclick="alert('Bottom Right Clicked!')"></a>
                </div>
            </td>
            <td>
                <div class="cell top-left">
                    <a href="#top-left" onclick="alert('Top Left Clicked!')"></a>
                </div>
                <div class="cell bottom-right">
                    <a href="#bottom-right" onclick="alert('Bottom Right Clicked!')"></a>
                </div>
            </td>
        </tr>
    </table>
</body>
</html>

