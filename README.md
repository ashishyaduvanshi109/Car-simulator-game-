# Car-simulator-game-
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Car Simulator Game Form</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to right, #1e1e1e, #ff0000);
      color: #fff;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      margin: 0;
    }

    .form-container {
      background: #111;
      padding: 30px 40px;
      border-radius: 20px;
      box-shadow: 0 0 20px rgba(255, 0, 0, 0.5);
      width: 90%;
      max-width: 500px;
    }

    h2 {
      text-align: center;
      margin-bottom: 25px;
      color: #ff5555;
    }

    label {
      display: block;
      margin-top: 15px;
      font-weight: bold;
    }

    input[type="text"],
    input[type="tel"],
    input[type="file"],
    textarea {
      width: 100%;
      padding: 10px;
      margin-top: 5px;
      background: #222;
      border: 1px solid #444;
      border-radius: 10px;
      color: #fff;
    }

    textarea {
      resize: vertical;
      height: 80px;
    }

    button {
      margin-top: 20px;
      width: 100%;
      padding: 12px;
      border: none;
      border-radius: 12px;
      background: #ff0000;
      color: #fff;
      font-size: 16px;
      font-weight: bold;
      cursor: pointer;
      transition: 0.3s ease;
    }

    button:hover {
      background: #cc0000;
    }

    .footer-text {
      text-align: center;
      margin-top: 10px;
      font-size: 13px;
      color: #ccc;
    }
  </style>
</head>
<body>
  <div class="form-container">
    <h2>Car Simulator Game</h2>
    <form action="https://formspree.io/f/your-form-id" method="POST" enctype="multipart/form-data">
      <label for="name">Name:</label>
      <input type="text" name="name" id="name" required />

      <label for="photo">Upload Your Photo:</label>
      <input type="file" name="photo" id="photo" accept="image/*" required />

      <label for="phone">Phone Number:</label>
      <input type="tel" name="phone" id="phone" pattern="[0-9]{10}" placeholder="10-digit number" required />

      <label for="document">Upload Document:</label>
      <input type="file" name="document" id="document" required />

      <label for="address">Address:</label>
      <textarea name="address" id="address" required></textarea>

      <button type="submit">Submit</button>
    </form>
    <div class="footer-text">
      Powered by Ashok Enterprises
    </div>
  </div>
</body>
</html>
