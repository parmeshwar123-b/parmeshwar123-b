<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Test</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <section>First section</section>

    <meta name="keyword" content="html, css, javascript">

    <iframe src="https://www.google.com" title="abccc" height="250px" width="250"></iframe>

    <h1>&#169; &lt; &amp;</h1>

    <p>div is a block-level element and span is an inline element</p>

    <audio src=""></audio>
    <video src=""></video>
    <header></header>
    <footer></footer>

    <a href="#" target="_self"></a>

    <form action="">
        <input type="radio" id="male" name="gender" value="male" checked>
        <label for="male">Male</label>
        <input type="radio" id="female" name="gender" value="female">
        <label for="female">Female</label>
        <input type="radio" id="other" name="gender" value="other">
        <label for="other">Other</label>
    </form>

    <!-- Commented out paragraph -->
    <!--<p></p>-->

    <label for="file">Choose a file</label>
    <input type="file" name="file" >

    <section>Second section</section>

    <div>
        <button onclick="geolocator()">Click to get location</button>
        <p id="paragraph"></p>
    </div>

    <script>
        let paragraph = document.getElementById("paragraph");
        let userLoc = navigator.geolocation;
        function geolocator() {
            if (userLoc) {
                userLoc.getCurrentPosition(success);
            } else {
                alert("Browser doesn't support geolocation API");
            }
        }
        function success(data) {
            let lat = data.coords.latitude;
            let long = data.coords.longitude;
            paragraph.innerHTML = "Latitude: " + lat + "<br>Longitude: " + long;
        }
    </script>

    <form action="#">
        Name: <input type="text" id="name" name="name" autofocus>
    </form>

    <!-- Questions and answers -->

    Q2: What is an attribute?
    Answer: An attribute is additional information about an HTML element or tag.

    Q4: Explain the use of the embed tag.
    Answer: The embed tag is used to embed external content, such as a plugin or a resource, into an HTML document.

    Q6: What is a formatting tag?
    Answer: A formatting tag is used to format the text in a webpage.

    Q5: Offline web page and manifest.
    Answer: <html manifest="demo.appcache"></html>

    <!-- To-do list application -->

    <h1>
        <input type="text" placeholder="Enter a task">
        <button>Add task</button>
        <ul>
            <li><task></task></li>
            <li><task></task></li>
            <li><task></task></li>
            <li><task></task></li>
            <li><task></task></li>
        </ul>
    </h1>

    <!-- Embed audio file -->

    <audio src="song.mp3" controls></audio>

    <!-- Form validation -->

    <form>
        Name: <input type="text" id="name" name="name" pattern="[A-Za-z]+">
        Email: <input type="email" id="email" name="email" pattern="[a-z0-9]+@gmail.com">
        Age: <input type="number" id="age" name="age" min="18" max="99">
        <input type="button" value="Submit">
    </form>

    <!-- Embed video -->

    <video src="video.mp4" controls></video>

    <!-- SVG example -->

    <svg width="100" height="100">
        <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow"/>
    </svg>

</body>
</html>
