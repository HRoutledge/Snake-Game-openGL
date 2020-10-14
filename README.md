After scraping my previous boids project I decided I would rather create a simple video game for my programming project. It was a slow and difficult problem due to technical difficulties, but unlike the previous project, this one is in a much more complete & functioning state. I was unable to get it 100% finished however the vast majority of what I set out to achieve has been completed. 

I used c++ (OOP), SDL, openGL to write the game. It is a simple game of snake. WASD controls the direction of the snake’s movement across a 30x30 grid, the perimeter of the grid is a wall that if the snake collides with, ends the game. Fruit is randomly placed inside the grid which results in the users score increasing when consumed. Lastly as the snake eats, it’s body grows in length making the gameplay more difficult and the likelihood of colliding with either a wall or the snake’s own body increase, which of course results in a gameover.

The grid/map is created using several nested for loops which use the grid width and height variables as a counter and populates each element of the grid with either a “#” representing a wall; “F” representing a fruit; “O” representing the snake; or a blank space showing the user where they can move. My aim was to then convert these grid elements to cubes of different colours and position them in the correct place. This is the only part of the project I was unable to successfully complete in time. The cubes are created as the loops are executed however there is no 3D position data or transformation matrix in place to correctly position them on the SDL window. So unfortunately they are all positioned in the centre. The console window is still created though which allows the user to play the game which is fully functional. Fixing this problem with the graphics shouldn’t be too difficult.

In regards to the openGL, there is a fully functional camera and lighting that can be adjusted in the code (as these are hard coded in and are not available for the user to edit) as well as the 3D objects being created and rendered as mentioned previously.

Overall, asides from the graphics being drawn in the incorrect place, I am quite happy with this project. It is a huge improvement over what I had made previously, I was still plagued with technical issues that made no sense such as SDL randomly stopping working requiring a full PC restart upon which it would start functioning as normal. These issues greatly slowed down the rate at which I was able to work on the project as this issue happened extremely frequently and I could not find what was causing the issue as there were no kind of error messages to speak of, it simply didn’t work (drew blank screen and stopped accepting keyboard input). 

###bibliography###

June 26 2017, javidx9, code it yourself snake! - Programming from scratch (Quick and Simple c++), UK,  (https://youtu.be/e8lYLYlrGLg)

A short YouTube tutorial series where user javidx9 goes over the process of creating several simple games in c++ using the console for output including snake, tetris and several others. Watching these helped give me an idea of how to implement ideas such as the game loop.

March 6 2018, Kate Gregory, c++17 Fundamentals, USA. (https://app.pluralsight.com/library/courses/cplusplus-fundamentals-c17/table-of-contents)
this was a very useful Pluralsight class that goes over much of modern c++ as well as some basic OOP/OOD theory. I used some of the OOP knowledge I gained from here when writing the snake code using classes & OOP.

Jun  13 2015, NVitanovic, c++ tutorial 18 - simple snake game, (https://www.youtube.com/watch?v=E_-lMZDi7Uw) 

Another short YouTube series similar to the first one referenced however this is slightly more in depth. I found this quite useful especially when trying to figure out how to implement the growth of the snake when it eats food as I was struggling with that.
