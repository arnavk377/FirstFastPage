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
    var name = ['Chrion', 'Camry', 'Model 48', 'Wraith'];
    var brand = ['Bugatti', 'Toyota', 'Ford', 'Rolls Royce'];
    var price = [3825000, 25945, 64995, 635000];
    var text = document.getElementById("text");
    var table = '<table><thead><tr><th>ID</th><th>Name</th><th>Brand</th><th>Price</th></tr></thead><tbody>';
    for(var i = 0; i < name.length; ++i) {
      const element_name = name[i]
      const element_brand = brand[i]
      const element_price = price[i]
      table += '<tr><td>' + (i + 1) + '</td><td>' + element_name + '</td><td>' + element_brand + '</td><td>' + element_price + '</td></tr>';
    }
    table += '</tbody></table>';

    text.innerHTML = table;

  </script>
</body>



