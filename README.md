# my-site-
﻿@{
    ViewData["Title"] = "Home Page";
}

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>@ViewData["Title"] - my_site</title>
    <link rel="stylesheet" href="~/lib/bootstrap/dist/css/bootstrap.min.css" />
    <style>
        body {
            background-image: url('sunset-8657085_640.jpg');
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            height: 100vh; /* Full height */
            margin: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: space-between;
        }

        .navbar {
            width: 100%;
            display: flex;
            justify-content: flex-start;
            padding: 10px 20px;
        }

            .navbar a {
                margin-right: 20px;
                color: black;
                text-decoration: none;
                font-weight: bold;
            }

                .navbar a:hover {
                    text-decoration: underline;
                }

        .container {
            text-align: center;
            color: blue;
        }

            .container h1 {
                margin-bottom: 20px;
            }

        .btn-primary, .btn-secondary {
            margin: 5px;
        }
    </style>
</head>
<body>
    
    <div class="container">
        <h1 class="display-4">Welcome to my site</h1>
        <p>
            <a class="btn btn-primary" asp-area="" asp-controller="Home" asp-action="Contact">Contact</a>
            <a class="btn btn-secondary" asp-area="" asp-controller="Home" asp-action="Resume">View My Resume</a>
        </p>
    </div>
    

    <script src="~/lib/jquery/dist/jquery.min.js"></script>
    <script src="~/lib/bootstrap/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
