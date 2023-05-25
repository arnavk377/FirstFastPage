---
toc: true
layout: post
description: Animation
categories: [markdown, ap]
title: Sprite
---

<html>
<head>
  <title>Sprite Animation Example</title>
  <style>
    .sprite {
      background-image: url('/Users/poonam/vscode/FirstFastPage/images/runnersprite.webp');
      background-repeat: no-repeat;
      height: 280px;  /* Adjust the height based on your sprite sheet */
      width: 65px;  /* Calculate the width based on the sprite sheet resolution and number of frames: 1040 / 16 = 65 */
      transform: scale(0.5);  /* Adjust the scale if needed */
      font-size: 2em;
      text-align: center;
    }

    #runner {
      background-position: 0px 0px;
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="row">
      <div class="column">
        <p class="sprite" id="runner" onmousedown="startAnimate('runner', 0, 0, 16)" onmouseover="stopAnimate('runner')">runner</p>
      </div>
    </div>
  </div>

  <script>
    var intervalIDs = {}; // Object to store interval IDs
    const pixels = 65; // Size of each frame in the sprite
    const interval = 100; // Animation time interval

    function startAnimate(id, row, col1, frames) {
      var col = col1; // Start at the first column/frame in the series of frames

      // Use the animation ID as the key for storing the interval ID
      intervalIDs[id] = setInterval(() => {
        /* Each pass sets the CSS backgroundPosition property to point to the next background frame
         * Formula: The row stays the same, but the column is mutated by adding 'pixels' each interval
         * Modulo Operator: 'frames * pixels' is the upper bound, 'col + pixels' is the increment,
         *                  and the remainder is the new column position
         * Offset: 'col1' is the offset of the first image in the series
         */
        document.getElementById(id).style.backgroundPosition = `-${col}px -${row}px`;
        col = (col + pixels) % (frames * pixels); // Use the modulo operator to cycle through the sequence
      }, interval); // Time interval
    }

    function stopAnimate(id) {
      // Stop the animation task ID
      clearInterval(intervalIDs[id]);
    }
  </script>
</body>
</html>
