g-support-
==========
<!doctype html>  
<html lang="en">  
<head>  
  <meta charset="utf-8">  
  <title>height demo</title>  
  <style>  
  body {  
    background: yellow;  
  }  
  button {  
    font-size: 12px;  
    margin: 2px;  
  }  
  p {  
    width: 150px;  
    border: 1px red solid;  
  }  
  div {  
    color: red;  
    font-weight: bold;  
  }  
  </style>  
  <script src="//code.jquery.com/jquery-1.10.2.js"></script>  
</head>  
<body>  
   
<button id="getp">Get Paragraph Height</button>  
<button id="getd">Get Document Height</button>  
<button id="getw">Get Window Height</button>  
   
<div>&nbsp;</div>  
<p>  
  Sample paragraph to test height  
</p>  
   
<script>  
function showHeight( element, height ) {  
  $( "div" ).text( "The height for the " + element + " is " + height + "px." );  
}  
$( "#getp" ).click(function() {  
  showHeight( "paragraph", $( "p" ).height() );  
});  
$( "#getd" ).click(function() {  
  showHeight( "document", $( document ).height() );  
});  
$( "#getw" ).click(function() {  
  showHeight( "window", $( window ).height() );  
});  
</script>  
   
</body>  
 </html>
