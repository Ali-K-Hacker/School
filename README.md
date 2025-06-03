<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>تسجيل الدخول</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: linear-gradient(135deg, #667eea, #764ba2);
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
    }

    .login-container {
      background-color: #fff;
      padding: 40px 30px;
      border-radius: 15px;
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
      max-width: 400px;
      width: 100%;
      text-align: center;
    }

    .login-container img {
      width: 60px;
      margin-bottom: 15px;
    }

    h2 {
      margin: 10px 0 15px;
      color: #333;
    }

    p {
      margin-bottom: 25px;
      color: #666;
      font-size: 14px;
    }

    input[type="text"],
    input[type="password"] {
      width: 100%;
      padding: 12px;
      margin-bottom: 20px;
      border: 1px solid #ccc;
      border-radius: 8px;
      font-size: 15px;
    }

    button {
      width: 100%;
      padding: 12px;
      background: linear-gradient(to right, #667eea, #764ba2);
      color: white;
      font-size: 16px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: background 0.3s ease;
    }

    button:hover {
      background: linear-gradient(to right, #5a67d8, #6b46c1);
    }
  </style>
</head>
<body>
  <div class="login-container">
    <img src="https://cdn-icons-png.flaticon.com/512/3064/3064197.png" alt="Lock Icon">
    <h2>تسجيل الدخول</h2>
    <p>يرجى إدخال بيانات الدخول للوصول إلى الموقع</p>
    <form>
      <input type="text" placeholder="اسم المستخدم" required>
      <input type="password" placeholder="كلمة المرور" required>
      <button type="submit">دخول</button>
    </form>
  </div>
</body>
</html>
