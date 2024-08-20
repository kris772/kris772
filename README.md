<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My JavaScript Counter</title>
</head>
<body>
    <p>Comment count: <span id="commentCount">0</span></p>

    <script>
        let commentCount = 0;
        const incrementBy = 10;

        // Simulate receiving comments (you can replace this with actual comment events)
        setInterval(() => {
            commentCount++;
            if (commentCount % 15 === 0) {
                const currentNumber = parseInt(document.getElementById('commentCount').textContent);
                document.getElementById('commentCount').textContent = currentNumber + incrementBy;
            }
        }, 1000); // Adjust the interval (in milliseconds) as needed.
    </script>
</body>
</html>
