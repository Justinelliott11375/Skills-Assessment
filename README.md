# Horton Skills Assessment
Copyright © 2018 Horton All rights reserved.

Objective
---------
Develop a webpage that matches the mockup in `./assets/mock.jpg`.

The website should:
  - Look as close to the mockup as possible on the latest versions of the browsers: Internet Explorer, Edge, Safari, Chrome, and Firefox at a screen width of 1920px.
  - Sections should animate in on scroll. This animation is up to you.
  - The hero image ( the image at the top of the page ) should randomly display one of the 3 hero images on page load.

Getting Started
---------------
1. Fork this repository
2. Make sure Node.js, NPM 5.6.0 and Gulp are installed
3. Run `npm init -y && npm install gulp && npm install gulp-sass gulp-autoprefixer browser-sync gulp-eslint gulp-concat gulp-uglify gulp-babel babel-core babel-preset-env gulp-rename @babel/core`
4. Run `gulp`

You can access the site at `localhost:3000`.

Colors
------
Black: #000\
White: #fff\
Red: #de041c

Fonts
-----
Montserrat\
https://fonts.google.com/specimen/Montserrat

Notes/Method
----------
Overall this project is not as responsive as what I would normally build. Pixels are used much more often than normal but knowing that the project is only meant to be viewed at a width of 1920px it didn't need to be responsive. I had a slight problem getting things set up. Simply running `npm install gulp` downloads gulp version 4 and the gulp tasks written for this project are in version 3. Reverting to version 3 solved the issue. Variables are used for colors. Obviously they don't need to be but this would allow for easier changes if the need should arise. Also had a small issue with the Montserrat font. From what I understand, Montserrat previously only had 2 weights: normal and bold(400 and 700) but some of the text appeared to be in Montserrat's black(900). I'm not sure if this was just by design in the test but my machine seemed to have the older version of Montserrat. I eventually solved this by downloading the additional styles that I believe have been out since 2017 but I did find some mention of similar issues with Google fonts online. Also ran into a problem with the hero image names. Again, I'm not sure if this was part of the test but I've never seen naming conventions that use spaces in file/image names. The image files would render when in my Sass file but I couldn't get them to load anywhere else. Changing the file name to include and underscore rather than a space solved this issue. No major problems but I did hit quite a few roadblocks. I built all the html first then started styling the header followed by the text on the right then the collage on the left. I had not used Sass, flexbox, animation, or CSS grids prior to this assignment so while there was quite a bit of new tech to be learned it was a lot of fun. Sass made styling organization a lot easier and flexbox simplified alignment. I think that the collage could have been done with flexbox, I'm not sure, but I had an easier time using CSS grid. the Collage itself is 3 seperate grids: one for the 2 images on the bottom left and one each for the left and right halves(counting the embedded video in the right half). The embedded video overlaps the header with a negative margin(and a subtle `box-shadow` I almsot missed). I'm sure there are multiple ways to animate the sections but using the `aos` tags seemed easiest. The text on the right is just a container to hold the background image with another div to align the text(which included a splash image I also almost missed).  The header was started first but finished last, I had a lot of issues with randomizing the hero images(it took me a while to decide it was OK to change the file names). I would have liked to use external javascript but had problems getting it to work without using it inline. I assume jQuery can make this easier but in the project itself its all inline, and unfortunately not being minified. Overall this project was a lot of fun and a great learning experience. I believe the site looks very similar to the mock-up albeit not as responsive as a live website would be.
