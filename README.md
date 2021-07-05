# assement
<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<style>
* {box-sizing: border-box}
body {font-family: "Lato", sans-serif;}

/* Style the tab */
.tab {
  float: left;
  border: 1px solid #ccc;
  background-color: #f1f1f1;
  width: 12%;
  height: 500px;
}

/* Style the buttons inside the tab */
.tab button {
  display: block;
  background-color: inherit;
  color: black;
  padding: 22px 16px;
  width: 100%;
  border: none;
  outline: none;
  text-align: left;
  cursor: pointer;
  transition: 0.3s;
  font-size: 17px;
}

/* Change background color of buttons on hover */
.tab button:hover {
  background-color: #ddd;
}

/* Create an active/current "tab button" class */
.tab button.active {
  background-color: #ccc;
}

/* Style the tab content */
.tabcontent {
  float: left;
  padding: 0px 12px;
  border: 1px solid #ccc;
  width: 70%;
  border-left: none;
  height: 500px;
}
.icon-bar  {
  display: block;
  text-align: left;
  padding: 16px;
  transition: all 0.3s ease;
  color:#4e3d36;
  width: 500px;
  font-size: 39px;
}
input {
  width: 50%;
}
</style>
</head>
<body>



<div class="tab">
  <div class="icon-bar">
<i class="fa fa-fw fa-home"></i></div>
  <button class="tablinks" onclick="openCity(event, 'Students')" id="defaultOpen"><i class="fa fa-fw fa-user"></i> Students</button>
  <button class="tablinks" onclick="openCity(event, 'Lesson Plan')"><i class="fa fa-fw fa-book"></i>Lesson Plan</button>
  <button class="tablinks" onclick="openCity(event, 'Settings')"><i class="fa fa-fw fa-cog">&nbsp;&nbsp;</i>Settings</button>
</div>

<div id="Students" class="tabcontent">
  <h3><B>Welcome</B></h3>
  <p>Amit Shinde</p>
</div>

<div id="Lesson Plan" class="tabcontent">
  <h3><B><i class="fa fa-fw fa-caret-left"></i>Videos</B></h3>
  <form action="/action_page.php"> &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;
  <label for="homepage"></label>
  <input type="url" id="homepage"  placeholder="Insert URl Here" name="homepage"><br><br>&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&nbsp;&nbsp;&nbsp;
  
</form><br><br>
<p align=center>or</p>
<form action="/action_page.php">&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;
 <label for="homepage"></label>
    
    <input type="submit" class="button" value="Upload">
</form>
<div class="video-display"></div>

</div>

<div id="Settings" class="tabcontent">
  <h3><B>Setting</B></h3>
  <p>This is setting of Video.</p>
</div>

<script>
function openCity(evt, cityName) {
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }
  document.getElementById(cityName).style.display = "block";
  evt.currentTarget.className += " active";
}

// Get the element with id="defaultOpen" and click on it
document.getElementById("defaultOpen").click();

 document.getElementById("myInputID").addEventListener("keyup", function(event) {
    if (event.keyCode === 13) {
    	document.getElementById("myFormID").submit();
		return false;
    }
}); document.getElementById("myInputID").addEventListener("keyup", function(event) {
    if (event.keyCode === 13) {
    	document.getElementById("myFormID").submit();
		return false;
    }
});
</script>
   
</body>
</html> 
