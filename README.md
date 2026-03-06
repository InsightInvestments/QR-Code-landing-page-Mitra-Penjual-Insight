<html>
<head>
  <title>QR Generator</title>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js"></script>
</head>
<body>
  <h2>QR Generator</h2>
  <input type="text" id="text" placeholder="https://insights.id/id/how-to-invest#partner">
  <button onclick="generateQR()">Generate</button>
  <div id="qrcode"></div>

  <script>
    function generateQR() {
      document.getElementById("qrcode").innerHTML = "";
      new QRCode(document.getElementById("qrcode"), {
        text: document.getElementById("text").value,
        width: 300,
        height: 300
      });
    }
  </script>
</body>
</html>
