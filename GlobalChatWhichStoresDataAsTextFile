<html>
<head>
  <style>
  body{
    margin: 0;
    background-color: #E2E2E2;
    font-family: Times New Roman;
  }
  #container{
    border: 2px solid black;
    width:300px;
    margin: auto;
    margin-top:20px;
    margin-bottom:20px;
    background-color: #444;
  }
  #_div{
    overflow-y: auto;
    overflow-x: hidden;
    max-width:100%;
    height: 350px;
    width: 300px;
  }
  #tx1{
    width: 225px;
    height: 50px;
    margin: 0;
    padding-left: 10px;
    border-top:2px solid black;
    font-size: 16px;
    font-family: Times New Roman;
  }
  #btn{
    width: 75px;
    height: 100px;
    margin: 0;
    float: right;
    border-top: 2px solid black;
    border-left: 2px solid black;
    font-family: Times New Roman;
    font-size: 16px;
  }
  p{
    margin-left: 10px;
    margin-right: 10px;
    padding: 10px;
    background-color: #CCC;
    border-radius: 10px;
  }
  #p1{
    background-color: #AAA;
    padding: 10px;
    margin: 0;
    border-top: 2px solid black;
    border-radius: 0;
  }
  h1{
    background-color: #AAA;
    margin: 0;
    padding: 10px;
    border-bottom:2px solid black;
  }
  span{
    color: red;
  }
  a{
    color: red;
  }
  </style>
</head>
<body>
<?php
if(isset ($_POST['text'])&& isset ($_POST['name']))
{
    $text = $_POST['text'];
    $name = $_POST['name'];
    $cloud = fopen('data.html', 'a');
    fwrite($cloud, "<p>" . $name . " : " . $text . "</p>");
    fclose($cloud);
}
?>
<div id="container">
<h1>Chat <span>Web</span> App</h1>
<div id="_div">
<?php
include "data.html" ;
?>
</div>
<form action="" method="POST">
<input type="text" id="tx1" placeholder="Enter your name (5 characters)" name="name" maxlength="5" required/>
<input type="submit" value="Send" id="btn"/>
<input type="text" id="tx1" placeholder="Enter a message (10 characters)" name="text" maxlength="10" required/>
</form>
<p id="p1">Developed by <a href=" gg ">Ahmed Saber</a></p>
</div>
<script>
    var element = document.getElementById("_div");
    element.scrollTop = element.scrollHeight;
    if ( window.history.replaceState ) {
        window.history.replaceState( null, null, window.location.href );
    }
</script>
</body>
</html>
