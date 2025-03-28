<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Subdomain Takeover</title>
    <style>
        body {
            background-color: black;
            color: #00ff00;
            font-family: 'Courier New', monospace;
            text-align: center;
            padding: 50px;
        }
        .glitch {
            font-size: 3em;
            font-weight: bold;
            text-transform: uppercase;
            position: relative;
            display: inline-block;
            animation: glitch 1s infinite;
        }
        @keyframes glitch {
            0% { text-shadow: 2px 2px red, -2px -2px blue; }
            50% { text-shadow: -2px -2px red, 2px 2px blue; }
            100% { text-shadow: 2px 2px red, -2px -2px blue; }
        }
        .terminal {
            background: rgba(0, 0, 0, 0.9);
            padding: 20px;
            border-radius: 10px;
            border: 2px solid #00ff00;
            display: inline-block;
            text-align: left;
            max-width: 600px;
        }
        .terminal p {
            margin: 5px 0;
            animation: blink 1s infinite alternate;
        }
        @keyframes blink {
            from { opacity: 1; }
            to { opacity: 0.3; }
        }
    </style>
</head>
<body>
    <h1 class="glitch">Subdomain Takeover</h1>
    <div class="terminal">
        <p>> Enumerating Subdomains...</p>
        <p>> Found: vulnerable.example.com</p>
        <p>> Checking CNAME records...</p>
        <p>> Takeover possible ✅</p>
        <p>> Deploying payload...</p>
        <p>> Access granted! 💀</p>
    </div>
</body>
</html>
