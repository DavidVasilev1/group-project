---
toc: true
comments: true
layout: post
title:  API Progress - Week 01
description: Summary of what we have done this week for our API and how we plan to progress with our API.
permalink: /api
categories: [Week 1]
---

<body>

  <p>Translate this page:</p>
  
  <div id="google_translate_element"></div>
  
  <script type="text/javascript">
  function googleTranslateElementInit() {
    new google.translate.TranslateElement({pageLanguage: 'en'}, 'google_translate_element');
  }
  </script>
  
  <script type="text/javascript" src="//translate.google.com/translate_a/element.js?cb=googleTranslateElementInit"></script>
  
  <p>You can translate the content of this page by selecting a language in the select box.</p>
  
</body>

# API 
To emphasize, as a backend developer, I constructed a data sheet full of plausible statistics for each ivy league college. The data was then transferred as an API through a CSV file, through this, we will now be able to integrate a calculator that bases off wether a student is eligible for any of these colleges through the data that is stored. 

![]({{site.baseurl}}/images/API.png)

ORIGINAL GOOGLE SHEET:
![]({{site.baseurl}}/images/debug3.png)

## Flask Issue
Currently we are trying to figure out why the table/API only works in the backend developer's personal flask, we tried to transfer it to our group's fastpages, but it kept on not working, we decided this will be our debugging issue. 

![]({{site.baseurl}}/images/debug1.png)
![]({{site.baseurl}}/images/debug2.png)

Above is the API, through table.html the table was imported under the templates folder in the flask. 
