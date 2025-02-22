# MindEaseAI 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MindEaseAI - AI-Powered Psychologist</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; padding: 50px; }
        #chatbox { width: 80%; max-width: 600px; margin: auto; padding: 10px; border: 1px solid #ccc; border-radius: 5px; }
        #userInput { width: 70%; padding: 8px; }
        #sendBtn { padding: 8px 15px; cursor: pointer; }
    </style>
</head>
<body>
    <h1>MindEaseAI - AI-Powered Psychologist</h1>
    <div id="chatbox">
        <p><strong>MindEaseAI:</strong> Hello! How can I help you today?</p>
    </div>
    <input type="text" id="userInput" placeholder="Type your message...">
    <button id="sendBtn">Send</button>

    <script>
        document.getElementById('sendBtn').addEventListener('click', function() {
            let userText = document.getElementById('userInput').value;
            if (userText.trim() !== "") {
                let chatbox = document.getElementById('chatbox');
                chatbox.innerHTML += `<p><strong>You:</strong> ${userText}</p>`;
                document.getElementById('userInput').value = "";
                
                // Simulated AI response
                setTimeout(() => {
                    let botReply = "I'm here to listen. Tell me more.";
                    chatbox.innerHTML += `<p><strong>MindEaseAI:</strong> ${botReply}</p>`;
                }, 1000);
            }
        });
    </script>
</body>
</html>
