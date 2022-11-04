---
title: Fetch of Backend Jokes
layout: default
description: An example of Frontend talking to Backend Python application serving jokes.  This example provides the ability to react to the Joke (haha or boohoo).
permalink: /data/jokes
image: /images/jokes.png
categories: [C4.7]
tags: [javascript, fetch, dom, getElementID, appendChild]
---


<!-- HTML table fragment for page -->
<table>
  <thead>
  <tr>
    <th>Name</th>
    <th>GPA</th>
    <th># of Extra Cirriculars</th>
    <th># of Leadership Positions</th>
    <th>White</th>
    <th>Hispanic</th>
    <th>African-American</th>
    <th>Asian</th>
    <th>Other</th>
    <th>Computer Science</th>
    <th>Business</th>
    <th>Biology</th>
    <th>Politics</th>
    <th>Engineering</th>
    <th>Social Sciences</th>
    <th>English</th>
    <th>Other</th>
    <th>Acceptance Rate</th>
    <th>SAT Score</th>
    <th>ACT Score</th>
    <th>Gender</th>
    <th>Essay</th>
  </tr>
</thead>
<tbody id="result">
    <!-- javascript generated data -->
</tbody>
</table>

<!-- Script is layed out in a sequence (without a function) and will execute when page is loaded -->
<script>

  // prepare HTML defined "result" container for new output
  const resultContainer = document.getElementById("result");

  // keys for joke reactions


  // prepare fetch urls
  const url = "https://sadv.nighthawkcodescrums.gq/api/college/";

  // prepare fetch GET options
  const options = {
    method: 'GET', // *GET, POST, PUT, DELETE, etc.
    mode: 'cors', // no-cors, *cors, same-origin
    cache: 'default', // *default, no-cache, reload, force-cache, only-if-cached
    credentials: 'omit', // include, *same-origin, omit
    headers: {
      'Content-Type': 'application/json'
      // 'Content-Type': 'application/x-www-form-urlencoded',
    },
  };
  // prepare fetch PUT options, clones with JS Spread Operator (...)
  const put_options = {...options, method: 'PUT'}; // clones and replaces method

  // fetch the API
  fetch(url, options)
    // response is a RESTful "promise" on any successful fetch
    .then(response => {
      // check for response errors
      if (response.status !== 200) {
          error('GET API response failure: ' + response.status);
          return;
      }
      // valid response will have JSON data
      response.json().then(data => {
          console.log(data);
          var order = ["college", "gpa", "ec", "award", "lead", "white", "hispanic", "africanamerican", "ec", "ec", "ec",]
          Object.entries(college_lists).sort((a, b) => order.indexOf(a) - order.indexOf(b)).forEach(([k, v]) => {

          })
          Object.entries(college_lists).forEach(([k, v]) => {
            console.log(row);

              // tr for each row
              const tr = document.createElement("tr");
              // td for each column
              const name = document.createElement("td");
              const cases = document.createElement("td");
              const deaths = document.createElement("td");
              const active = document.createElement("td");

              // data is specific to the API
              name.innerHTML = row.country_name;
              cases.innerHTML = row.cases; 
              deaths.innerHTML = row.deaths; 
              active.innerHTML = row.active_cases; 

              // this builds td's into tr
              tr.appendChild(name);
              tr.appendChild(cases);
              tr.appendChild(deaths);
              tr.appendChild(active);

              // add HTML to container
              resultContainer.appendChild(tr);
          })
      })
  })
  // catch fetch errors (ie Nginx ACCESS to server blocked)
  .catch(err => {
    error(err + " " + url);
  });

  // Something went wrong with actions or responses
  function error(err) {
    // log as Error in console
    console.error(err);
    // append error to resultContainer
    const tr = document.createElement("tr");
    const td = document.createElement("td");
    td.innerHTML = err;
    tr.appendChild(td);
    resultContainer.appendChild(tr);
  }

</script>