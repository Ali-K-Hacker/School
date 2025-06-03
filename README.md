<html lang="ar" dir="rtl">
<head>
    <meta name="generator" content="none">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>تسجيل الدخول</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #000000 100%);
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 20px;
            position: relative;
        }

        /* المستطيل العلوي الجديد */
        .top-cover {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 60px;
            background: linear-gradient(135deg, #667eea 0%, #000000 100%);
            z-index: 1;
        }

        /* كلمة School الجديدة - معدلة */
        .school-title {
            position: absolute;
            top: 15px;
            left: 20px;
            color: white;
            font-size: 30px;
            font-weight: bold;
            z-index: 2;
        }

        .login-container {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
            width: 100%;
            max-width: 400px;
            text-align: center;
            border: 1px solid rgba(255, 255, 255, 0.2);
            z-index: 0;
        }

        .login-header {
            margin-bottom: 30px;
        }

        .login-header h1 {
            color: #000000;
            font-size: 28px;
            margin-bottom: 10px;
            font-weight: 600;
        }

        .login-header p {
            color: #666;
            font-size: 16px;
        }

        .form-group {
            margin-bottom: 20px;
            text-align: right;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            color: #555;
            font-weight: 500;
            font-size: 14px;
        }

        .form-group input {
            width: 100%;
            padding: 15px;
            border: 2px solid #e1e5e9;
            border-radius: 10px;
            font-size: 16px;
            transition: all 0.3s ease;
            background: rgba(255, 255, 255, 0.9);
            text-align: right;
        }

        .form-group input:focus {
            outline: none;
            border-color: #667eea;
            box-shadow: 0 0 0 3px rgba(102, 126, 234, 0.1);
            background: white;
        }

        .login-btn {
            width: 100%;
            padding: 15px;
            background: linear-gradient(135deg, #6a8cff 0%, #4a6bff 100%);
            border: none;
            border-radius: 10px;
            color: white;
            font-size: 16px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            margin-top: 10px;
        }

        .login-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 25px rgba(102, 126, 234, 0.3);
        }

        .access-btn {
            width: 100%;
            padding: 18px;
            background: linear-gradient(135deg, #00b894 0%, #00a085 100%);
            border: none;
            border-radius: 12px;
            color: white;
            font-size: 18px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            margin-bottom: 15px;
            box-shadow: 0 5px 15px rgba(0, 184, 148, 0.3);
        }

        .access-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 25px rgba(0, 184, 148, 0.4);
        }

        .logout-btn {
            width: 100%;
            padding: 12px;
            background: linear-gradient(135deg, #fd79a8 0%, #e84393 100%);
            border: none;
            border-radius: 8px;
            color: white;
            font-size: 14px;
            font-weight: 500;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .logout-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 20px rgba(232, 67, 147, 0.3);
        }

        .error-message {
            background: #ffe6e6;
            color: #d63031;
            padding: 12px;
            border-radius: 8px;
            margin-top: 15px;
            border: 1px solid #fab1a0;
            display: none;
            font-size: 14px;
        }

        .info-box {
            background: rgba(0, 184, 148, 0.1);
            border: 1px solid rgba(0, 184, 148, 0.3);
            border-radius: 10px;
            padding: 15px;
            margin-top: 20px;
            color: #00b894;
            font-size: 14px;
            text-align: center;
        }

        .lock-icon {
            font-size: 48px;
            color: #667eea;
            margin-bottom: 20px;
        }

        .success-icon {
            font-size: 48px;
            color: #00b894;
            margin-bottom: 20px;
        }

        .buttons-container {
            margin: 30px 0;
        }

        @media (max-width: 480px) {
            .login-container {
                padding: 30px 20px;
            }
        }
    </style>
</head>
<body>
    <div class="top-cover"></div>
    <div class="school-title">School</div>
    
    <div class="login-container" id="loginPage">
        <div class="login-header">
            <div class="lock-icon">🔒</div>
            <h1>تسجيل الدخول</h1>
            <p>يرجى إدخال بيانات الدخول للوصول إلى الموقع</p>
        </div>
        
        <form id="loginForm">
            <div class="form-group">
                <label for="username">اسم المستخدم:</label>
                <input type="text" id="username" name="username" required>
            </div>
            
            <div class="form-group">
                <label for="password">كلمة المرور:</label>
                <input type="password" id="password" name="password" required>
            </div>
            
            <button type="submit" class="login-btn">دخول</button>
        </form>
        
        <div id="errorMessage" class="error-message">
            اسم المستخدم أو كلمة المرور غير صحيحة
        </div>
    </div>

    <div class="login-container" id="welcomePage" style="display: none;">
        <div class="login-header">
            <div class="success-icon">✅</div>
            <h1>مرحباً بك!</h1>
            <p>تم تسجيل الدخول بنجاح</p>
        </div>
        
        <div class="buttons-container">
            <button class="access-btn" id="accessSite">
                🌐 دخول الموقع الرئيسي
            </button>
            
            <button class="logout-btn" id="logoutBtn">
                🚪 تسجيل خروج
            </button>
        </div>
        
        <div class="info-box">
            <p>اضغط على "دخول الموقع الرئيسي" للوصول إلى المحتوى</p>
        </div>
    </div>

    <script>
        const VALID_USERNAME = "school";
        const VALID_PASSWORD = "2030";
        const PROTECTED_SITE_URL = "https://sites.google.com/view/md7turki/%D8%A7%D9%84%D8%B5%D9%81%D8%AD%D8%A9-%D8%A7%D9%84%D8%B1%D8%A6%D9%8A%D8%B3%D9%8A%D8%A9?authuser=0";

        const loginPage = document.getElementById('loginPage');
        const welcomePage = document.getElementById('welcomePage');
        const loginForm = document.getElementById('loginForm');
        const errorMessage = document.getElementById('errorMessage');
        const accessBtn = document.getElementById('accessSite');
        const logoutBtn = document.getElementById('logoutBtn');

        loginForm.addEventListener('submit', function(e) {
            e.preventDefault();
            
            const username = document.getElementById('username').value;
            const password = document.getElementById('password').value;
            
            if (username === VALID_USERNAME && password === VALID_PASSWORD) {
                loginPage.style.display = 'none';
                welcomePage.style.display = 'block';
            } else {
                errorMessage.style.display = 'block';
                
                setTimeout(() => {
                    errorMessage.style.display = 'none';
                }, 3000);
                
                document.getElementById('username').value = '';
                document.getElementById('password').value = '';
            }
        });

        accessBtn.addEventListener('click', function() {
            window.open(PROTECTED_SITE_URL, '_blank');
        });

        logoutBtn.addEventListener('click', function() {
            welcomePage.style.display = 'none';
            loginPage.style.display = 'block';
            
            document.getElementById('username').value = '';
            document.getElementById('password').value = '';
        });
    </script>
</body>
</html>
