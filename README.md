# codewithChetan
#FrontENDCODE
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login Page</title>
    
<body style="background-color:#d2bea5;">
    <img src="myjpurney.jpg"  align="left" valign="center" alt="Logo" width=850 height=800  style="margin:20px;">
    <div class="login-container" style="background-color:rcba(255,255,255,1);;">
        <div class="left-panel">
            <br>
            <br>
            <br>
            <br>
            <br>
            <br>
            <br>
            <br>
            <br>
            <h1 style="text-align:center-right; font-size: xx-large;">Welcome To <i><b>myjourney</b></i></h1><br><br>
            <p>Please sign in to your account.</p>
        </div>
        <div class="right-panel">
            <form>
                <h2>Sign in</h2>
                <input type="email" placeholder="Email or Username" name="email" required>
                <input type="password" placeholder="password" name="password" required>
                <button type="submit"><a href="file:///C:/Users/WELCOME/OneDrive/Desktop/NEW/Homepage.html">Login</a></button>
            </form>
            <div class="options">
                <label for="remember-me">Remember Me</label>
                <input type="checkbox" id="remember-me">
                <a href="#">Forgot password?</a>
            </div>
            <div class="social-login">
                <span>Or sign in with</span> 
                <div class="social-buttons">
                    <button class="facebook"><a href="https://www.facebook.com/"><img src="facebook.jpg" width="25" height="25"></a></button>
                    <button class="google"><a href="https://www.google.com/"><img src="google.jpg" width="25" height="25"></a></button>
                </div>
            </div>
            <p>Don't have an account? <a href="file:///C:/Users/WELCOME/OneDrive/Desktop/NEW/Form.html">Sign up</a></p>
            
        </div>
    </div>
    </body>
</html>

#HOMEPAGECODE
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <style>
        .rd{background-color:rgba(244, 245, 245, 0.5);
            border:10px;

    box-sizing:border-box;
    text-align:center;

margin-top:200px;
margin-bottom:500px;
margin-left:500px;
margin-right:500px;
padding:10px}
    </style>
</head>
<body  background="1080p.webp" style="background-color:bisque;">
    <div class="rd">
                <h1><u><i>Plan Your Trip</i></u></h1>
                <h2><u>Details</u></h2>
                <div><p>Name: <input type="Name" placeholder="Name"></p>
                <p>Contact: <input type="Contact" placeholder="Mobile no."></p>
                <p>E-mail: <input type="E-mail" placeholder="E-mail"></p>
                <p>Location: <input type="Location" placeholder="Location"></p>
                <p>Days: <input type="Days" placeholder="Days"></p>
                </p>
                <p>Budget: <input type="Budget" placeholder="Budget"></p>
                </div>
                <h3>Additional Details</h3>
                <div><p>Number of people Traveling: <input type="No." placeholder="No."></p>
                    <h1>Participants Name, Age, Gender</h1>
    
                    <form id="participant-form">
                        <input type="text" id="participant-name" placeholder="Participant Name">
                        <button type="button" onclick="addParticipant()">Name,Age,Gender</button>
                    </form>
                
                    <ul id="participant-list">
                    </ul>
                
                    <script>
                        function addParticipant() {
                            const nameInput = document.getElementById("participant-name");
                            const name = nameInput.value; 
                
                            if (name.trim() !== "0") {
                                const list = document.getElementById("participant-list");
                                const listItem = document.createElement("li")
                                listItem.textContent = name;
                                list.appendChild(listItem);
                
                                nameInput.value = "";
                            }
                        }
                    </script>
                </div>
    </div></body>
</html>


#FORMCODE
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>Registration Form</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <h1>Registration Form</h1>
    <p>Please fill out this form with the required information</p>
    <form method="post" action='new.html'>
      <fieldse t>
        <label for="first-name">Enter Your First Name: <input id="first-name" name="first-name" type="text" required /></label>
        <label for="last-name">Enter Your Last Name: <input id="last-name" name="last-name" type="text" required /></label>
        <label for="email">Enter Your Email: <input id="email" name="email" type="email" required /></label>
        <label for="new-password">Create a New Password: <input id="new-password" name="new-password" type="password" min="6" max="20" required /></label>
      </fieldset>
      <fieldset>
        <legend>Nationality</legend>
        <label for="indian"><input id="indian" type="radio" name="account-type" class="inline" checked />Indian</label>
        <label for="foreigner"><input id="foreigner" type="radio" name="account-type" class="inline" />Foreigner</label>
      </fieldset>
      <fieldset>
        <label for="profile-picture">Upload a profile picture: <input id="profile-picture" type="file" name="file" /></label>
        <label for="proof">Enter your Identity Form:<input id="proof" type="file" name="file"></label>
        <label for="age">Input your age (years): <input id="age" type="number" name="age" min="13" max="120" /></label>
        <label for="referrer">How did you hear about us?
          <select id="referrer" name="referrer">
            <option value="">(select one)</option>
            <option value="1">from recommandation</option>
            <option value="2">from advertisement</option>
            <option value="3">from self research </option>
            <option value="4">Other</option>
          </select>
        </label>
        <label for="bio">Provide a bio:
          <textarea id="bio" name="bio" rows="3" cols="30" placeholder="I would like to tell you more about....."></textarea>
        </label>
      </fieldset>
      <label for="terms-and-conditions"> I accept the <a href="terms and conditions.html">terms and conditions</a>
        <input id="terms-and-conditions" type="checkbox" required name="terms-and-conditions" />
      </label>
      <a href="new.html">
      <input type="submit" value="Submit" /></a>
    </form>
  </body>
</html>



#STYLECSS
body {
    width: 100%;
    height: 100vh;
    margin: 0;
    background-color: #1b1b32;
    color: #f5f6f7;
    font-family: Tahoma;
    font-size: 16px;
  }
  
  h1, p {
    margin: 1em auto;
    text-align: center;
  }
  
  form {
    width: 60vw;
    max-width: 500px;
    min-width: 300px;
    margin: 0 auto;
    padding-bottom: 2em;
  }
  
  fieldset {
    border: none;
    padding: 2rem 0;
    border-bottom: 3px solid #3b3b4f;
  }
  
  fieldset:last-of-type {
    border-bottom: none;
  }
  
  label {
    display: block;
    margin: 0.5rem 0;
  }
  
  input,
  textarea,
  select {
    margin: 10px 0 0 0;
    width: 100%;
    min-height: 2em;
  }
  
  input, textarea {
    background-color: #0a0a23;
    border: 1px solid #0a0a23;
    color: #ffffff;
  }
  
  .inline {
    width: unset;
    margin: 0 0.5em 0 0;
    vertical-align: middle;
  }
  
  input[type="submit"] {
    display: block;
    width: 60%;
    margin: 1em auto;
    height: 2em;
    font-size: 1.1rem;
    background-color: #3b3b4f;
    border-color: white;
    min-width: 300px;
  }
  
  input[type="file"] {
    padding: 1px 2px;
  }


