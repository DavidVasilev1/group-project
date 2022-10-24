---
toc: false
comments: true
layout: post
title:  User Interface
description: The Project's UI
permalink: /project
categories: [Week 1]
---

# Input your academic traits below. 
# --------------------------------

<!-- This here is the code for a dropdown menu regarding genders.  -->
<html>
<script>
function gen() {
    var genderList = document.getElementById("genderList");
    document.getElementById("gender").innerHTML = genderList.options[genderList.selectedIndex].text;
  }
</script>
<body>
<!-- Here below are the options from which the inputter may choose from.  -->
<form>
Please Select Your Gender:
<select id="genderList" onchange="gen()">
    <option> ---Choose Gender--- </option>  
    <option> Male </option>  
    <option> Female </option>  
</select>

<p>Your selected gender is: <font color = "#ffffc2"><t id = "gender"></t></font></p>
</form>

</body>
</html>


<!-- This here is the code for a dropdown menu regarding numerous ethnicities.  -->
<html>
<script>
function eth()
{
var ethnicityList=document.getElementById("ethnicityList");
document.getElementById("ethnicity").innerHTML=ethnicityList.options[ethnicityList.selectedIndex].text;
}
</script>
<body>
<!-- Here below are the options from which the inputter may choose from.  -->
<form>
Please Select Your Ethnicity:
<select id="ethnicityList" onchange="eth()">
    <option> ---Choose Ethnicity--- </option>  
    <option> White </option>  
    <option> Hispanic </option>  
    <option> African-American </option>  
    <option> Asian </option>  
    <option> Other </option>  
</select>
<p>Your selected ethnicity is: <font color = "#ffffc2"><t id = "ethnicity"></t></font></p>
</form>

</body>
</html>




<!-- This here is the code for a dropdown menu regarding numerous majors.  -->
<html>
<script>
function maj()
{
var majorList=document.getElementById("majorList");
document.getElementById("major").innerHTML=majorList.options[majorList.selectedIndex].text;
}
</script>
<body>
<form>
<!-- Here below are the options from which the inputter may choose from.  -->
<html>
Please Select Your Major:
<select id="majorList" onchange="maj()">
    <option> ---Choose Major--- </option>  
    <option> Computer Science </option>  
    <option> Business </option>  
    <option> Biology </option>  
    <option> Politics </option>  
    <option> Engineering </option>  
    <option> Social Sciences </option>
    <option> English </option>
    <option> Other </option>
</select>
<p>Your selected major is: <font color = "#ffffc2"><t id = "major"></t></font></p>








<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>

<body>
  <label> Enter your GPA</label><br>
  <input type = "text" id = "gpa"><br>
  <button type="button" id="gpabutton">submit</button>

  <script src="script.js">
  </script>
  <script>

document.getElementById("gpabutton").onclick = function(){

    var gpa = document.getElementById("gpa").value;
    console.log("Your GPA is ",gpa);
}
</script>
</body>
</html>
<p>Your GPA is: <font color = "#ffffc2"><t id = "gpa"></t></font></p>









<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>

<body>
  <label> Enter the amount of extracurriculars you are a part of</label><br>
  <input type = "text" id = "ec"><br>
  <button type="button" id="ecbutton">submit</button>

  <script src="script.js">
  </script>
  <script>

document.getElementById("ecbutton").onclick = function(){

    var ec = document.getElementById("ec").value;
    console.log("This is how many extracurriculars you are part of: ",ec);
}
</script>
</body>
</html>
<p>This is how many extracurriculars you are part of: <font color = "#ffffc2"><t id = "ec"></t></font></p>








<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>

<body>
  <label> Enter the amount of awards you have won</label><br>
  <input type = "text" id = "awards"><br>
  <button type="button" id="awardbutton">submit</button>

  <script src="script.js">
  </script>
  <script>

document.getElementById("awardbutton").onclick = function(){

    var award = document.getElementById("ec").value;
    console.log("This is how many awards you have won: ",ec);
}
</script>
</body>
</html>
<p>This is how many awards you have won: <font color = "#ffffc2"><t id = "award"></t></font></p>






<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>

<body>
  <label> Enter the amount of leadership positions you have</label><br>
  <input type = "text" id = "lead"><br>
  <button type="button" id="leadbutton">submit</button>

  <script src="script.js">
  </script>
  <script>

document.getElementById("leadbutton").onclick = function(){

    var lead = document.getElementById("lead").value;
    console.log("This is how many leadership positions you have: ",lead);
}
</script>
</body>
</html>
<p>This is how many leadership positions you have: <font color = "#ffffc2"><t id = "lead"></t></font></p>




<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>

<body>
  <label> Enter your SAT score (if applicable)</label><br>
  <input type = "text" id = "SAT"><br>
  <button type="button" id="SATbutton">submit</button>

  <script src="script.js">
  </script>
  <script>

document.getElementById("SATbutton").onclick = function(){

    var SAT = document.getElementById("SAT").value;
    console.log("Your SAT score is: ",SAT);
}
</script>
</body>
</html>
<p>Your SAT score is: <font color = "#ffffc2"><t id = "SAT"></t></font></p>






<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>

<body>
  <label> Enter your ACT score (if applicable)</label><br>
  <input type = "text" id = "ACT"><br>
  <button type="button" id="ACTbutton">submit</button>

  <script src="script.js">
  </script>
  <script>

document.getElementById("ACTbutton").onclick = function(){

    var ACT = document.getElementById("ACT").value;
    console.log("Your ACT score is: ",ACT);
}
</script>
</body>
</html>
<p>Your ACT score is: <font color = "#ffffc2"><t id = "ACT"></t></font></p>




<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>

<body>
  <label> Enter your essay grade </label><br>
  <input type = "text" id = "essay"><br>
  <button type="button" id="essaybutton">submit</button>

  <script src="script.js">
  </script>
  <script>

document.getElementById("essaybutton").onclick = function(){

    var essay = document.getElementById("essay").value;
    console.log("Your essay grade is: ",essay);
}
</script>
</body>
</html>
<p>Your essay grade is: <font color = "#ffffc2"><t id = "essay"></t></font></p>



<button>Calculate</button>
