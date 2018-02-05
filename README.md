**Frontend-nanodegree-mobile-portfolio project**
**Udacity Front-end Nanodegree Program**
Test this with [Page](https://rcheng709.github.io/frontend-nanodegree-mobile-portfolio/).

##To Build Project Locally
-Fork the repo from Udacity, clone the repo, and navigate to its root directory
-It took me a while because I have to install Python, NodeJs and Ngrok so I can run Google Page insight.
-Once I have changed the Environment variables in my PC, I was able to run Page Insight.
-Using the command prompt in my PC
 *$> cd /path/to/your-project-folder*
 *$> python.exe -m http.server 8080 (my Python version is 3.6)*

 *Open another terminal or command prompt:*
 *$> cd /path/to/your-project-folder*
 *$> ngrok http 8080*

**Note: When you run ngrok, make sure to take note the forwarding server, this is your gateway for the Page Insight to analyze your website.**
-Example:
-Forwarding                    https://5abcde80.ngrok.io -> localhost:8080

SHORTENING THE CRITICAL RENDERING PATH
•	added async attribute to the google analytics script and js/perfmatters.js
•	added media="print" to the css/print link to unblock critical rendering path
•	inlined styles in index.html from style.css file
•	moved script files down below the body of the html
•	optimized pizzeria, cam_be_like, mobilewebdev profilepic images using website http://tinyjpg.com
PIZZERIA
•	changed the items[i].style.left to transform and transalte to improve FPS
•	moved the items variable down below the anonymous function that generates the sliding pizzas
•	also made the items variable available globally by adding window.items = document.querySelectorAll('.mover');
•	implemented requestAnimationFrame as described in http://www.html5rocks.com/en/tutorials/speed/animations/
•	 removed the dx variable declaration from the changePizzaSizes function for loop
•	removed document.querySelector("#movingPizzas1") from the event listener anonymous function and into its own variable 
GRUNT
•	Install Node Js, Grunt in project directory
•	Install grunt plugin ‘grunt-contrib-cssmin’ and create gruntfile.js to customize task to minify css files in views/css

