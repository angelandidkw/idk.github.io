<html>

<head>
    <title>Interactive Website</title>
    <style>
        #content {
            text-align: center;
        }
    #image {
            width: 200px;
            transition: width 0.5s ease;
        }
        .button {
            border: none;
            color: white;
            padding: 16px 32px;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            margin: 4px 2px;
            transition-duration: 0.4s;
            cursor: pointer;
        } 
        #noButton {
            background-color: #008CBA;
            border: 2px solid #008CBA;
        }
        #noButton:hover {
            background-color: #004466;
            border: 2px solid #004466;
        }
        #yesButton {
            background-color: #04AA6D;
            border: 2px solid #04AA6D;
        }
        #yesButton:hover {
            background-color: #00663e;
            border: 2px solid #00663e;
        }
        #thankYouMessage {
            display: none;
        }
    </style>
</head>

<body>
    <div id="content">
        <h1>Do you like this image?</h1>
        <img id="image" src="https://github.com/angelandidkw/websiteme.github.io/assets/148724145/aac13686-39a2-4142-8691-cd495cf2711f" alt="Cute Kitten">
        <br>
        <button id="noButton" class="button" onclick="makeBigger()">No</button>
        <button id="yesButton" class="button" onclick="sayThankYou()">Yes</button>
        <div id="thankYouMessage"></div>
    </div>

<script>
        function makeBigger() {
            var image = document.getElementById('image');
            var currentWidth = image.offsetWidth;
            image.style.width = (currentWidth + 50) + 'px';
        }

        function sayThankYou() {
            var content = document.getElementById('content');
            var thankYouMessage = document.getElementById('thankYouMessage');

            // Replace the content with a big "Thank You" image
            content.innerHTML = '<img src="https://github.com/angelandidkw/websiteme.github.io/assets/148724145/9c149110-e51f-42e6-9a81-18eb0ab8e0d2" alt="Big Thank You Image">';
        }
    </script>
</body>

</html>
