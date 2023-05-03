Download Link: https://assignmentchef.com/product/solved-cs2261-lab6-usenti-and-spritesheets
<br>
In this lab, you’ll be familiarizing yourself with Usenti by creating your own spritesheet. Your completed Lab 6 should display a screen with a message using the sprites you’ve drawn in Usenti. Each TODO represents a component of this lab, and is broken down into sub-TODOs. Your code may not compile until you complete an entire TODO block, at which point the game should compile with the new drawing function working as expected. Complete the TODOs in order, paying close attention to the instructions. ​<strong>For this lab, it is important you follow instructions on where to place sprites in your spritesheet. </strong>Precision is necessary.

Note: Make sure to copy over your Makefile and .vscode/tasks.json from one of your previous assignments.

<strong>TODO 1.0 – Usenti </strong>

The majority of this lab is going to take place in Usenti. You will be creating a spritesheet with the 26 ​<em>capital</em>​ letters of the alphabet. You will also be making a custom sprite of your choosing.

<ul>

 <li>Make sure to familiarize yourself with the Usenti cheatsheet located in Canvas under Files &gt; Recitations &gt; Usenti.</li>

 <li>Open Usenti, go to Image &gt; Size, and change the size to 256 x 256. Click “Stretch”, then “OK”.</li>

 <li>You can keep the color of the canvas as black, or you can change it to another color. Make sure that none of your sprites contain the same color as the background of your spritesheet.

  <ul>

   <li>If you want to change the color, click on the color picker, then on the canvas, then go to the color editor on the right side and change the color.</li>

  </ul></li>

 <li>Now it is time to add your letter sprites. The sprites <strong>must</strong>​ follow the same size,​            format, and orientation as described here, or your lab will not work properly.

  <ul>

   <li>Each of your letter sprites must be 2×2 tiles. Use the tile grid tool to make sure your letter sprites fit within this size.</li>

  </ul></li>

</ul>

○ They can be any color except black and the color of your spritesheet background.

○ Your spritesheet must contain all 26 capital alphabets, from A-Z, in order.

○ You can draw each letter using the pencil tool, or you can use the text tool to type them onto the spritesheet. If you use the text tool, you can use any color or font, but make sure that the font size is big enough to fill out the 2×2 tile size, but not too big that it goes past the boundaries set by the grid.

○ Your letter sprites should be placed in the following way on your spritesheet,

○

where A starts at the very top of your spritesheet (column = 0, row = 0), B starts at the next 2 tiles (column = 2, row = 0), and so on and so forth until P, which is drawn at the last 2×2 space in that row. Q is then drawn two tiles below A.

○ Use the rectangular selection tool to move your sprites around to ensure that they are centered in their 2×2 space.

○ Go to Palette &gt; Requantize, and change the number of colors to the minimum number of colors used in your spritesheet. For example, in the example spritesheet above only magenta and white are used, so the palette would be requantized to 2.

<ul>

 <li>Next, you should draw your custom sprite. This can be anything you want, but you must make sure that its size is roughly 4×4 tiles, or 32×32 pixels. Again you can check this using the tile grid or pixel grid in Usenti.

  <ul>

   <li>You can draw this in Usenti, or you can find a picture online that you want to use.</li>

  </ul></li>

</ul>

■ <strong>If you use a picture you found online</strong>, you should open it using a​         separate Usenti window, resize it to 32×32 pixels (make sure to click “Stretch”). Requantize your image’s palette to (16 – number of colors in your spritesheet’s palette).

■ Go to Image &gt; Export, and export your image as a palette. Click OK for the Palette Exporter pop-up.

■ Now in your spritesheet Usenti window, go to Image &gt; Import, click your image’s palette. Source should be 0, Dest should be the next empty index in your spritesheet’s palette. For example, if my spritesheet’s palette has only 2 colors, Dest would be the next empty index which is 2. Count should be the number of colors you are importing, i.e. the number of colors in your image’s palette. Click OK.

■ Go back to your image’s Usenti window, select it using the rectangular tool, then copy using keyboard shortcuts and paste it onto your spritesheet’s Usenti window. Your image’s colors should still look the same, if not, you did not import the palette correctly.

■ Make sure your image has the same background color as your spritesheet. Use the color picker to select a pixel from your image’s background, and change it to match your spritesheet’s background color.

■ Also, <strong>make sure</strong>​          the first color (or zero-th index) in your spritesheet’s​     palette is the background color (aka the “transparent” color). If it is not, use the palette swap tool by referencing the Usenti cheatsheet.

<strong>■ If you draw your own custom sprite,</strong> make sure you click on the​          next empty index in your spritesheet’s palette and change the color to whatever color you’d like to use. Make sure that the number of colors in your spritesheet’s palette does not go above 16.

○ Your custom sprite should start in the row right after Q (column = 0, row = 4), and should span 4 tiles horizontally and 4 tiles vertically. Here is how your spritesheet should look:




<ul>

 <li>Your spritesheet is now done. Now export your spritesheet as a GBA source, making sure to name it “spritesheet” and to check the correct options in the exporter for Mode 0 (use the Usenti cheatsheet for help). Then, also export as a Windows bitmap, making sure to click 4 for “bit depth” when prompted.</li>

</ul>

<strong>○ Note: </strong>If there are problems with loading your spritesheet into the GBA​  screen, re-export your spritesheet in Usenti and make sure to not check “reduce” under “Map” when exporting as a GBA source.

<strong>TODO 2.0- Loading your spritesheet </strong>

<ul>

 <li>TODO 2.1: Include the relevant .h files at the top of your main.c file</li>

 <li>TODO 2.2: Use DMA to load in the spritesheet tiles into the corresponding charblock and the spritesheet palette into the sprite palette. Remember, this is Mode 0.</li>

 <li>Run your lab. If the screen displays “CONGRATS” in your spritesheet’s letters and then displays your custom sprite right below that, you are done. Good job!</li>

</ul>




<strong> </strong>




<h1>Tips</h1>

<ul>

 <li>Review lecture and recitation materials for how we deal with Mode 0 sprites</li>

 <li>Review how to use Usenti to export spritesheets</li>

 <li>Follow each TODO in order, and only move forward if everything is correct</li>

</ul>


