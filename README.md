# passwordStrengthMeter
A Simple Password Strength Meter Based On zxcvbn.js

## Usage

```
<html lang="en">
<head>
  <link rel="stylesheet" href="path/to/passwordStrengthMeter.min.css">
</head>
<body>
  
  <div>
    <h5>Password:</h5>
    <input name="password" type="password" placeholder="*****" required />
    <span class="password-meter"></span>
  </div>
    
  ....
  
  <script src="path/to/jquery.js"></script>
  <script src="path/to/jquery.passwordStrengthMeter.min.js"></script>
  <script>
      $(function() {
        $(".password-meter").passwordStrengthMeter({
            passwordInput: "input[name=password]",
            // ratings: ["Very Weak", "Weak", "OK", "Strong", "Very Strong"], optional
            // allProgressBarClasses: "password-meter-very-weak password-meter-weak password-meter-ok  password-meter-strong  password-meter-very-strong", //optional
            // progressBarClasses: ["password-meter-very-weak","password-meter-weak","password-meter-ok","password-meter-strong","password-meter-very-strong"],
        }); //optional
      });
  </script>
</body>
</html>

```
