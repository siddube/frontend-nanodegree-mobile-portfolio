# Running the Application

Clone the GitHub repository

`$ git clone https://github.com/siddube/frontend-nanodegree-mobile-portfolio.git`

Open Index.html with a web browser (eg.Chrome, Firefox) to start the application.

# Steps Taken for Optimizing main.js for pizza.html
1. Save the value of document.body.scrollTop value in a variable and avoiding an FSL by calling the variable instead of document.body.scrollTop. This makes sure that the scrolling runs at 60FPS.

2. Save value of document.querySelectorAll(".randomPizzaContainer") in a variable and use the variable instead of calling document.querySelectorAll(). Use the value size in switch to assign the correct width upon changing pizza size. This takes care of the FSL and the change happens way under 5ms.

