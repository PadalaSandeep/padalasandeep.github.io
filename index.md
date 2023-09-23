<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kushi's Diet Plan</title>
    <!-- Include Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <!-- Custom CSS for table -->
    <style>
        body {
            background-color: #f5f5f5; /* Light background color */
        }

        .table-container {
            overflow-x: auto; /* Enable horizontal scrolling on smaller screens */
            max-width: 100%;
        }

        table {
            border-collapse: collapse;
            width: 100%;
            max-width: 1200px; /* Adjust as needed for larger screens */
        }

        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: center;
        }

        th {
            font-weight: bold;
        }
    </style>
        <script>
        // Hide the h1 tag content when the page loads
        window.addEventListener('load', function () {
            var h1Tag = document.querySelector('h1');
            if (h1Tag) {
                h1Tag.style.display = 'none';
            }
        });
    </script>
</head>
<body>
    <div class="container">
        <h1 class="text-center">Diet Plan</h1>
        <table class="table table-bordered">
            <thead>
                <tr>
                <th>Days</th>
                    <th>Early Morning</th>
                    <th>Morning (Eat a bit heavy as you need more energy for the day)</th>
                    <th>Afternoon</th>
                    <th>Night</th>
                </tr>
            </thead>
            <tbody>
                <!-- 10 rows of diet plan -->
                <tr>
                <td>1</td>
                    <td>Walking, Excersie and Yoga (15 mints each). Have a tulasi green tea</td>
                    <td>
                    Ragi dosa, ABC(Apple, Beetroot, Carrot Juice)
                    </td>
                    <td>Rice, Dal, Ghee, your fav fry and curd</td>
                    <td>Keep diet very light and eat lots of fruits (Apple would be great)</td>
                </tr>
                <tr>
                <td>2</td>
                    <td>Walking, Excersie and Yoga (20 mints each). Have a tulasi green tea</td>
                    <td>
                    Idli and wada, Carrot Juice
                    </td>
                    <td>Rice, Tomato curry, (Every first Mudha with kaaram and Ghee), your fav fry and curd</td>
                    <td>Keep diet very light and eat lots of fruits (Apple would be great)</td>
                </tr>
                                <tr>
                <td>3</td>
                    <td>Walking, Excersie and Yoga (25 mints each). Have a tulasi green tea</td>
                    <td>
                   Carrot Dosa, Beetroot Juice
                    </td>
                    <td>Rice, Dal, Ghee, your fav fry and curd</td>
                    <td>Keep diet very light and eat lots of fruits (Apple would be great)</td>
                </tr>
                                <tr>
                <td>4</td>
                    <td>Walking, Excersie and Yoga (25 mints each). Have a tulasi green tea</td>
                    <td>
                    Ragi dosa, ABC(Apple, Beetroot, Carrot Juice)
                    </td>
                    <td>Rice, Mixed vegetable curry, Ghee, your fav fry and curd</td>
                    <td>Keep diet very light and eat lots of fruits (Apple would be great)</td>
                </tr>
                
                            <tr>
                <td>5</td>
                    <td>Walking, Excersie and Yoga (30 mints each). Have a tulasi green tea</td>
                    <td>
                    Your fav Upma(eeee), ABC(Apple, Beetroot, Carrot Juice)
                    </td>
                    <td>Veg Biryani and curd</td>
                    <td>Keep diet very light and eat lots of fruits (Apple would be great)</td>
                </tr>
            </tbody>
        </table>
    </div>

    <!-- Include Bootstrap JS and jQuery (for Bootstrap functionality) -->
    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.3/dist/umd/popper.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
</body>
</html>
