---
toc: true
layout: post
description: HTML and Javascript Table
categories: [week5, csp, js]
image: 
title: HTML and JS Table
---

<head>
  <title>Table</title>
</head>
<body>
  <div id = "text"></div>
  <script>
    var cars = [{name: "Chrion", brand: "Bugatti", price: "$3825000"}, 
    {name: "Camry", brand: "Toyota", price: "$25945"},
    {name: "Model 48", brand: "Ford", price: "$64995"},
    {name: "Wraith", brand: "Rolls Royce", price: "$635000"}];
    
    var table = '<table><thead><tr><th>ID</th><th>Name</th><th>Brand</th><th>Price</th></tr></thead><tbody>';
    for(var i = 0; i < cars.length; i++) {
      const element_name = cars[i].name
      const element_brand = cars[i].brand
      const element_price = cars[i].price
      table += '<tr><td>' + (i + 1) + '</td><td>' + element_name + '</td><td>' + element_brand + '</td><td>' + element_price + '</td></tr>';
    }
    table += '</tbody></table>';

    text.innerHTML = table;

  </script>
</body>



