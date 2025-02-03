<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chat with Your GF</title>
    <style>
        body { font-family: Arial, sans-serif; }
        #chat-box { width: 100%; height: 300px; overflow-y: scroll; border: 1px solid #ccc; margin-bottom: 10px; }
        #message { width: 80%; padding: 5px; }
        button { width: 15%; padding: 5px; }
        h2 { text-align: center; }
    </style>
</head>
<body>
    <h2>Chat with Your GF</h2>
    <div id="chat-box"></div>
    <input type="text" id="message" placeholder="Type a message...">
    <button onclick="sendMessage()">Send</button>

    <!-- Start of Tawk.to Script -->
    <script type="text/javascript">
    var Tawk_API = Tawk_API || {}, Tawk_LoadStart = new Date();
    (function () {
        var s1 = document.createElement("script"), s0 = document.getElementsByTagName("script")[0];
        s1.async = true;
        s1.src = 'https://embed.tawk.to/67a126593a84273260795ab9/1ij6nrjit';
        s1.charset = 'UTF-8';
        s1.setAttribute('crossorigin', '*');
        s0.parentNode.insertBefore(s1, s0);
    })();
    </script>
    <!-- End of Tawk.to Script -->

    <script>
        function sendMessage() {
            const message = document.getElementById("message").value;
            if (message) {
                const chatBox = document.getElementById("chat-box");
                const newMessage = document.createElement("div");
                newMessage.innerText = message;
                chatBox.appendChild(newMessage);
                document.getElementById("message").value = ""; // clear input
                chatBox.scrollTop = chatBox.scrollHeight; // scroll to the bottom
            }
        }
    </script>
</body>
</html>
