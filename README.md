# Password Strength Meter
A Simple Password Strength Meter Based On zxcvbn.js

## Dependencies
- jQuery 1.7+

** No need to Pull in zxcvbn.js as the plugin pulls it in, by default, hence the reason for the large file size.**

## Usage

```html
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
        $(".password-meter").passwordStrengthMeter(); 
      });
  </script>
</body>
</html>

```

## Options

```javascript
$(function() {

 var $userInputs = [
    $('input[name=email]').val(),
    $('input[name=firstName]').val(),
 ];
 
  $(".password-meter").passwordStrengthMeter({
      passwordInput: "input[name=password]",
      userInputs: $userInputs,
      ratings: ["Very Weak", "Weak", "OK", "Strong", "Very Strong"],
      allProgressBarClasses: "password-meter-very-weak password-meter-weak password-meter-ok  password-meter-strong  password-meter-very-strong",
      progressBarClasses: ["password-meter-very-weak","password-meter-weak","password-meter-ok","password-meter-strong","password-meter-very-strong"],
  }); 
});

```
