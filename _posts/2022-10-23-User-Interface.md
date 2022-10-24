---
toc: false
comments: true
layout: post
title:  User Interface
description: The Project's UI
permalink: /project
categories: [Week 1]
---

# Please input your academic traits and essay grade. 
# .


<html>
<script>
function gen()
{
var genderList=document.getElementById("genderList");
document.getElementById("gender").value=genderList.options[genderList.selectedIndex].text;
}
</script>
<body>
<form>
Please Select Your Gender:
<select id="genderList" onchange="gen()">
    <option> ---Choose Gender--- </option>  
    <option> Male </option>  
    <option> Female </option>  
</select>
<p>Your selected gender is: <input type = "text" id = "gender" size = "20"></p>
</form>

</body>
</html>



<html>
<script>
function eth()
{
var ethnicityList=document.getElementById("ethnicityList");
document.getElementById("ethnicity").value=ethnicityList.options[ethnicityList.selectedIndex].text;
}
</script>
<body>
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
<p>Your selected ethnicity is: <input type = "text" id = "ethnicity" size = "20"></p>
</form>

</body>
</html>



<html>
<script>
function maj()
{
var majorList=document.getElementById("majorList");
document.getElementById("major").value=majorList.options[majorList.selectedIndex].text;
}
</script>
<body>
<form>
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
<p>Your selected major is: <input type = "text" id = "major" size = "20"></p>
</form>

</body>
</html>

