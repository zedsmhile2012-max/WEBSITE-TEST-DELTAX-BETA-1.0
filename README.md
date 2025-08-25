<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Prank Button</title>
<style>
  body, html {
    margin: 0;
    padding: 0;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: Arial, sans-serif;
    background-color: #f0f0f0;
    transition: background-color 0.5s;
  }
  .box {
    background-color: #fff;
    padding: 40px;
    text-align: center;
    border-radius: 10px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.3);
  }
  button {
    padding: 10px 20px;
    font-size: 16px;
    cursor: pointer;
    border: none;
    background-color: #007bff;
    color: white;
    border-radius: 5px;
  }
  button:hover {
    background-color: #0056b3;
  }
  #message {
    display: none;
    color: white;
    font-size: 48px;
    text-align: center;
  }
</style>
</head>
<body>
<div class="box" id="box">
  <h2>Press the Button</h2>
  <button onclick="prank()">Press Me</button>
</div>

<div id="message">YOU ARE GAY 😎</div>

<script>
function prank() {
  // Hide the box
  document.getElementById('box').style.display = 'none';
  // Change background to black
  document.body.style.backgroundColor = 'black';
  // Show the message
  document.getElementById('message').style.display = 'block';
}
</script>
</body>
</html>
