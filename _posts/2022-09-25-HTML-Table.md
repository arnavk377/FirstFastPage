---
toc: true
layout: post
description: HTML and Javascript Table
categories: [markdown, week4, csp, js]
image: 
title: HTML and JS Table
---

<script>
function dealership(name, brand, price) {
    this.name = name;
    this.brand = brand;
    this.price = price;
}

var students = [ 
    new dealership("Chrion", "Bugatti", 3,825,000),
    new dealership("Camry", "Toyota", 25,945),
    new dealership("Model 48(From 1935)", "Ford", 64,995),
    new dealership("Wraith", "Rolls Royce", 635,000),
];

table.prototype._toHtml = function() {
  // HTML Style is build using inline structure
  var style = (
    "display:inline-block;"
  );

  // HTML Body of Table is build as a series of concatenations (+=)
  var body = "";
  // Heading for Array Columns
  body += "<tr>";
  body += "<th><mark>" + "Car Name" + "</mark></th>";
  body += "<th><mark>" + "Brand" + "</mark></th>";
  body += "<th><mark>" + "Price" + "</mark></th>";
  body += "</tr>";
  // Data of Array, iterate through each row of compsci.classroom 
  for (var row of dealership) {
    // tr for each row, a new line
    body += "<tr>";
    // td for each column of data
    body += "<td>" + row.name + "</td>";
    body += "<td>" + row.brand + "</td>";
    body += "<td>" + row.price + "</td>";
    // tr to end line
    body += "<tr>";
  }

   // Build and HTML fragment of div, table, table body
  return (
    "<div style='" + style + "'>" +
      "<table>" +
        body +
      "</table>" +
    "</div>"
  );


};

function myFunction() {
  document.getElementById("mine").style.fontSize = "35px"; 
  document.getElementById("mine").style.color = "blue";       
}

$$.html(dealership._toHtml());

</script>



<center><button type="button" onclick="myFunction()" style="background: red">Click Me!</button></center>
