# Class-Site
<!DOCTYPE html>
<html lang="eng">
<head>
  <meta charset="utf-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <!-- The above 3 meta tags *must* come first in the head; any other head content must come *after* these tags -->
  <title>Homework</title>
  <!-- Bootstrap -->
  <link href="bootstrap-3.3.5-dist/css/bootstrap.min.css" rel="stylesheet">
  <link href="stylesheets/305.css" rel="stylesheet">
  <script src="https://cdn.firebase.com/js/client/2.2.1/firebase.js"></script>
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>
  <!--<script src="javascripts/snowstorm.js"></script>-->
  <!-- for the Snowstorm homepage, allow the demo to run on iPhone and mobile devices. -->
  <!--<script>snowStorm.excludeMobile = false;</script>-->
  <!--<script>snowStorm.followMouse = false;</script>-->
  <!-- HTML5 shim and Respond.js for IE8 support of HTML5 elements and media queries -->
  <!-- WARNING: Respond.js doesn't work if you view the page via file:// -->
  <!--[if lt IE 9]>
      <script src="https://oss.maxcdn.com/html5shiv/3.7.2/html5shiv.min.js"></script>
      <script src="https://oss.maxcdn.com/respond/1.4.2/respond.min.js"></script>
    <![endif]-->
</head>
<body background="images/BKG3.jpg">
    <nav class="navbar navbar-inverse navbar-fixed-top">
      <div class="container">
        <div class="navbar-header">
          <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#navbar" aria-expanded="false" aria-controls="navbar">
            <span class="sr-only">Toggle navigation</span>
            <span class="icon-bar"></span>
            <span class="icon-bar"></span>
            <span class="icon-bar"></span>
          </button>
          <a class="navbar-brand" href="./index.html">305</a>
        </div>
        <div id="navbar" class="collapse navbar-collapse">
          <ul class="nav navbar-nav">
            <li class="active"><a href="./index.html">Homework</a></li>
             <li><a href="./fun.html">Fun Stuff</a></li> 
            
             <li><a href="./monster.html">Monster Projects</a></li>
            <li><a href="./newspaper.html">Newspaper</a></li>
            <li><a href="./books.html">Book Stuff</a></li>
            <li><a href="./feedback.html">Feedback</a></li>
           <!-- <li><a href="#contact">Contact</a></li> -->
          </ul>
        </div><!--/.nav-collapse -->
      </div>
    </nav>

    <br>
    <br>
    <br>
    <h1>Welcome back to school!</h1>
    <br>
    Extreme passwords goes as the following (CASE AND SPACE SENSETIVE!): <br>
    <br>
    smep?s <br>
    THE END <br>
    Jimmy <br>
    12/19/15 <br>
    <br>
    And the fifth one is for you to figure out! <br>
    <br>
    Also, the secret password is omegaflowiePie135
    <br>
    <br>
   		



             <script>
var rubric = document.getElementById("r");
rubric.onclick = function(){
  location.href="./rubric.html"
}
    </script>

<!-- <input type='password' id='passInput' placeholder='Secret Password'> -->
<a href="https://classof20181.appspot.com/" class="btn btn-primary"><span class="glyphicon glyphicon-lock"></span> Click here to go to secret password</a>
<script>

   
</script>
<br>
<br>

<br>
<a class="btn btn-danger" role="button" id="btn">Pointless Button</a>
<script>
var counts = {},
    track  = document.getElementsByClassName('btn btn-danger');

for (var i = 0, max = track.length; i < max; i++) {
    track[i].addEventListener('click', function() {
        // Caching...
        var name = this.name,
            ele  = document.getElementById(name + '-count') || false;
        
        // Check if the array index exists, if it doesn't create it with a value
        // of '0' by default
        if (typeof counts[name] === 'undefined') {
            counts[name] = 1;
        }

            
      //   if (counts[name] == 100) {
      //   alert("Achievement Get: POINTLESS! (to go to secret webpage, press OK)");
      //   location.href = './secretyoucantrememberthis9873217337128312371902731.html'
      // }

        
        
        // Check if the element exists, if it doesn't create it
        if (!ele) {
            var ele    = document.createElement('div');
                ele.id = name + '-count';
            
            // Insert the new element after the next sibling so it falls after this
            // element in the DOM
            this.parentNode.insertBefore(ele, this.nextSibling);
        }

        
        ele.innerHTML = counts[name]++;
    });
}
</script>
<script> var x = new Firebase('https://sizzling-fire-7530.firebaseio.com/Button');

x.on('value', function f(s) {
    $('#counting').text(0 + s.val());
});

$('#btn').click(function() {
  x.transaction(function(current_value) {
    return current_value + 1;
  });
});

$('#reset').click(function() {
    x.set(0);
});
</script>
<h1>This button has been clicked <div id="buttontext">150106 times</div>
</h1> 
<script>
kemp="";
var ref3 = new Firebase("https://sizzling-fire-7530.firebaseio.com/Button");
    ref3.on("value", function(snapshot) {
      kemp = snapshot.val() + "";
      var btn = document.getElementById("buttontext");
      btn.innerHTML = kemp.concat(" times");
      });
</script>



       
    <!-- jQuery (necessary for Bootstrap's JavaScript plugins) -->
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.3/jquery.min.js"></script>
    <!-- Include all compiled plugins (below), or include individual files as needed -->
    <script src="bootstrap-3.3.5-dist/js/bootstrap.min.js"></script>
  

</body>

</html>
