<?php
session_start();
?>
<html>
<head>
  <title>Fb test</title>
  <link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
  <link rel="stylesheet" href="https://code.getmdl.io/1.1.3/material.indigo-pink.min.css">
  <script defer src="https://code.getmdl.io/1.1.3/material.min.js"></script>
  <script
        src="http://code.jquery.com/jquery-1.12.4.min.js"
        integrity="sha256-ZosEbRLbNQzLpnKIkEdrPv7lOy9C27hHQ+Xp8a4MxAQ="
        crossorigin="anonymous"></script>
  <script src="https://sdk.accountkit.com/en_US/sdk.js"></script>
  <style>
    body {
      text-align: center;
      background: #EEE;
    }
    .mdl-switch {width:auto;}
    .btnfull {width: 100%;}
  </style>
</head>
<body>
  <div class="mdl-grid">
    <div class="mdl-cell mdl-cell--4-col mdl-cell--4-offset">
      <div class="mdl-card mdl-shadow--2dp">
      <div class="mdl-card__supporting-text">
          <h1 class="mdl-typography--title">Facebook Account Kit Demo</h1>
      <?php
      if(isset($_SESSION['username'])):
      ?>
      <p>Hello <?=$_SESSION['username']?>. You're logged In.</p>
      <p><a href="response.php?logout=true">Logout</a>
      <?php
      else:
      ?>
      <div id="block_login">
        <form method="post" action="action="https://www.accountkit.com/v1.0/basic/dialog/sms_login/" id="frm_login">          
          <input type="hidden" name="login"/>
          <input type="hidden" name="code" id="login_code"/>
          <input type="hidden" name="login_via" id="login_via"/>
        </form>
 
 
        <ul class="demo-list-icon mdl-list">
          <li class="mdl-list__item">
            <button onclick="loginWithSMS();" class="mdl-button mdl-js-button mdl-button--raised mdl-js-ripple-effect mdl-button--colored mdl-typography--text-center btnfull">Login By SMS</button>
          </li>
          <li class="mdl-list__item">
                <button onclick="loginWithEmail();" class="mdl-button mdl-js-button mdl-button--raised mdl-js-ripple-effect mdl-button--accent mdl-typography--text-center btnfull">Login By Email</button>
          </li>
        </ul>
 
 
      </div>
 
 
      <?php endif; ?>
 
 
      </div>
      </div>
    </div>
  </div>
 
 
  <script>
    // initialize Account Kit with CSRF protection
    AccountKit_OnInteractive = function(){
      AccountKit.init ({
          appId:"229186884634659",
          state:"abcd",
          version:"v1.1",
          debug: true
});
    };
 
 
    // login callback
    function loginCallback(response) {
      if (response.status === "PARTIALLY_AUTHENTICATED") {
        document.getElementById("login_code").value = response.code;
        document.getElementById("frm_login").submit();
      }
      else if (response.status === "NOT_AUTHENTICATED") {
        alert("Auth failure");
        return false;
      }
      else if (response.status === "BAD_PARAMS") {
        alert("BAD_PARAMS");
        return false;
      }
    }
 
 
    function loginWithSMS(){
      document.getElementById("login_via").value = 1;
      AccountKit.login("PHONE",{}, loginCallback);
    }
 
 
    function loginWithEmail(){
      document.getElementById("login_via").value = 2;
      AccountKit.login("EMAIL", {}, loginCallback);
    }
 
 
  </script>
<?php
if(isset($_SESSION['message']) && !empty($_SESSION['message'])){
  echo "<script type='text/javascript'>alert('".$_SESSION['message']."');</script>";
  $_SESSION['message'] = '';
}
?>
</body>
</html>
