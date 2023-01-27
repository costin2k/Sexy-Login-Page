
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login</title>
    <link rel="stylesheet" href="style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat&display=swap" rel="stylesheet">
</head>

<body>
    <div class="container">
        <h1>Login</h1>
        <form method="post">
            <div class="text-field">
                <input type="text" required>
                <span></span>
                <label>Username</label>
            </div>

            <div class="text-field">
                <input type="password" required>
                <span></span>
                <label>Password</label>
            </div>

            <div class="pass">Forgot Password?</div>
            <input type="submit" value="Login">

            <div class="signup_link">Not a member? <a href="#">Signup</a> </div>



        </form>




    </div>

</body>

</html>

* {
    box-sizing: border-box;
}

html,
body {
    height: 100%;
    width: 100%;
}

body {
    margin: 0;
    padding: 0;
    font-family: 'Montserrat', sans-serif;
    background: linear-gradient(120deg, #2980b9, #8e44ad);
    overflow: hidden;
    font-weight: 600;
}


.container {
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    background-color: white;
    width: 400px;
    border-radius: 10px;
}

.container h1 {
    text-align: center;
    padding: 0 0 20px 0;
    border-bottom: 1px solid silver;
}


.container form {
    margin: 0 40px;

}

.text-field {
    position: relative;
    border-bottom: 1px solid silver;
    margin: 30px 0 30px;
}

.text-field input {
    width: 100%;
    height: 40px;
    padding: 0 5px;
    font-size: 16px;
    border: none;
    outline: none;
}

.text-field label {
    position: absolute;
    left: 5px;
    top: 50%;
    color: #adadad;
    pointer-events: none;
    transform: translateY(-50%);

}

.text-field span::before {
    content: '';
    position: absolute;
    top: 40px;
    left: 0;
    width: 100%;
    height: 2px;
    background: #2691d9;
}


.text-field input:focus~label,
.text-field input:valid~label {
    top: -5px;
    color: #2691d9;
    transition: 0.5s;
}


.pass {
    margin: -5px 0 20px 5px;
    color: #adadad;
    cursor: pointer;

}

.pass:hover {
    text-decoration: underline;
}

.pass input {
    border-color: #2691d9;
    transition: .5s;
}


input[type="submit"] {
    width: 100%;
    height: 50px;
    background-color: #2691d9;
    border: none;
    border-radius: 25px;
    font-size: 18px;
    color: #e9f4fb;
    cursor: pointer;
    outline: none;


}

input[type="submit"]:hover {
    border-color: #2691d9;
    transition: .5s;
}


.signup_link {
    margin: 30px 0;
    text-align: center;
    font-size: 16px;
    color: #666666;
}

.signup_link a {
    color: #2691d9;
    text-decoration: none;
}

.signup_link a:hover {
    text-decoration: underline;
}
