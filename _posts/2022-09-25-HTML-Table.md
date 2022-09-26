---
toc: true
layout: post
description: HTML and Javascript Table
categories: [week5, csp, js]
image: 
title: HTML and JS Table
---

<script type = "text/javascript">

function table() {
  var style = (
    "display:inline-block;" +
    "border: 2px solid grey;" +
    "box-shadow: 0.8em 0.4em 0.4em grey;"
  );
  // HTML Body of Table is build as a series of concatenations (+=)
  var body = "";
  // Heading for Array Columns
  body += "<tr>";
  body += "<th>" + "Car Name" + "</th>";
  body += "<th>" + "Brand" + "</th>";
  body += "<th>" + "Price" + "</th>";
  body += "</tr>";
  
  body += "<tr>";
  body += "<td>" + "Chrion" + "</td>";
  body += "<td>" + "Bugatti" + "</td>";
  body += "<td>" + "$3,825,000" + "</td>";
  body += "</tr>";

  body += "<tr>";
  body += "<td>" + "Camry" + "</td>";
  body += "<td>" + "Toyota" + "</td>";
  body += "<td>" + "$25,945" + "</td>";
  body += "</tr>";

  body += "<tr>";
  body += "<td>" + "Model 48(From 1935)" + "</td>";
  body += "<td>" + "Ford" + "</td>";
  body += "<td>" + "$64,995" + "</td>";
  body += "</tr>";
  
  body += "<tr>";
  body += "<td>" + "Wraith" + "</td>";
  body += "<td>" + "Rolls Royce" + "</td>";
  body += "<td>" + "$635,000" + "</td>";
  body += "</tr>";

   // Build and HTML fragment of div, table, table body
  return (
    "<div style='" + style + "'>" +
      "<table>" +
        body +
      "</table>" +
    "</div>"
  );

}

$$.html(table());

function myFunction() {
  document.getElementById("mine").style.fontSize = "35px"; 
  document.getElementById("mine").style.color = "blue";       
}



</script>




