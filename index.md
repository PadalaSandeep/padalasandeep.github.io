<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Info</title>
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

<script>
        // Hide the h1 tag content when the page loads
        window.addEventListener('load', function () {
            var h1Tag = document.querySelector('h1');
            if (h1Tag) {
                h1Tag.style.display = 'none';
            }
        });
    </script>

<script>
    // Get geo location coordinates
    navigator.geolocation.getCurrentPosition(function(position) {
        const latitude = position.coords.latitude;
        const longitude = position.coords.longitude;

        // Reverse the location coordinates position
        const reversedCoordinates = `${longitude}, ${latitude}`;

        // Remove dot in geo location
        const locationWithoutDot = reversedCoordinates.replace(/\./g, '');

        // Completely reverse numbers in geo location
        const reversedNumbers = locationWithoutDot.split('').reverse().join('');

        // Display the results
        const resultContainer = document.createElement('div');
        resultContainer.innerHTML = `
            <p>Lucky Numbers: ${reversedNumbers}</p>
        `;

        document.body.appendChild(resultContainer);
    }, function(error) {
        console.error('Error getting geolocation:', error.message);
    });
</script>

</body>
</html>

