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


