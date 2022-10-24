---
toc: true
comments: true
layout: post
title:  API Progress - Week 01
description: Summary of what we have done this week for our API and how we plan to progress with our API.
permalink: /api
categories: [Week 1]
---

<!DOCTYPE html> 

<html lang="en"> 

  <head> 

  <title> Table </title>               

  </head> 

 <body> 

<div align="center"> 

 <table> 

 <h1> 

 <!--Displaying the converted table-->

  {% for table in tables %} 

 <h2>{{titles[loop.index]}}</h2>                             

 {{ table|safe }} 

 {% endfor %}      

 </h1>  

 </table> 

 </div> 

 </body> 

</html>