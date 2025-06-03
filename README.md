<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>تسجيل الدخول</title>
  <link href="https://fonts.googleapis.com/css2?family=Cairo&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Cairo', sans-serif;
      background: linear-gradient(135deg, #6e8efb, #a777e3);
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .login-box {
      background: white;
      padding: 40px 30px;
      border-radius: 15px;
      box-shadow: 0 10px 30px rgba(0,0,0,0.1);
      width: 100%;
      max-width: 400px;
    }

    h2 {
      margin-bottom: 25px;
      color: #333;
    }

    .input-group {
      position: relative;
      margin-bottom: 20px;
    }

    input[type="text"], input[type="password"] {
      width: 100%;
      padding: 12px 15px;
      border: 1px solid #ccc;
      border-radius: 10px;
      font-size: 16px;
      outline: none;
      transition: 0.3s;
    }

    input[type="text"]:focus, input[type="password"]:focus {
      border-color: #6e8efb;
      box-shadow: 0 0 5px rgba(110, 142, 251, 0.5);
    }

    .toggle-password {
      position: absolute;
      top: 50%;
      left: 10px;
      transform: translateY(-50%);
      cursor: pointer;
      font-size: 18px;
      color: #888;
    }

    button {
      width: 100%;
      padding: 12px;
      border: none;
      background: #6e8efb;
      color: white;
      font-size: 16px;
      border-radius: 10px;
      cursor: pointer;
      transition: 0.3s;
    }

    button:hover {
      background: #5a76f3;
    }
  </style>
</head>
<body>
  <div class="login-box">
    <h2>تسجيل الدخول</h2>
    <form>
      <div class="input-group">
        <input type="text" placeholder="اسم المستخدم" required>
      </div>
      <div class="input-group">
        <input type="password" placeholder="كلمة المرور" id="password" required>
        <span class="toggle-password" onclick="togglePassword()">👁️</span>
      </div>
      <button type="submit">دخول</button>
    </form>
  </div>

  <script>
    function togglePassword() {
      const passwordInput = document.getElementById("password");
      const icon = document.querySelector(".toggle-password");
      if (passwordInput.type === "password") {
        passwordInput.type = "text";
        icon.textContent = "🙈";
      } else {
        passwordInput.type = "password";
        icon.textContent = "👁️";
      }
    }
  </script>
</body>
</html>
