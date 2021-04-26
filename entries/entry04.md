# Entry 4
##### 4/25/21

I am now working on my freedom project using my IDE. I have also created a repository for the project on my [github](https://github.com/ivanc4515/SEP11FP) page. My goal now is to create my MVP of the project. I have simplified my project to be a single game of plinko. I chose the game plinko because it utilizes a lot of the things I can do using Matter. As of right now I have completed the background of the plinko game. This includes the walls, dots, separators, and the ball that will drop. One of the problems I ran into while creating the background was the repetition. In plinko games there are many dots to act as obstacles for the ball to reach the bottom. Since each dot has their own unique position you have to create each and every dot. One Solution I wanted to implement was to create a function that would have a for loop to create the dot and simply alter the position. Instead of making the function for the dots I started small and tried to apply the same thing but for the separators at the bottom.
```
function separators(){
    var posX = 180
    for (var i=4; i == 0; i--){
      var separator = Bodies.rectangle(posX, 580, 10, 100, {
        isStatic: true
        });     
        console.log(posX)
        posX += 160;
        World.add(engine.world,[separator])
    };
};
```
As you can see the idea was that when the function separators() was called it would loop the creations of the separators. The following image shows the original lines of code. 
```
var separator1 = Bodies.rectangle(180, 580, 10, 100, {
    isStatic: true
});
var separator2 = Bodies.rectangle(340, 580, 10, 100, {
    isStatic: true
});
var separator3 = Bodies.rectangle(500, 580, 10, 100, {
    isStatic: true
});
var separator4 = Bodies.rectangle(660, 580, 10, 100, {
    isStatic: true
});
```
In my Engineering Design Process I am at a 5(Create a prototype) and 6 (Test and evaluate the prototype). I know what the plan is and I'm scheduling what I will do next to not pile up work. Next I will work on user input and allow the user to choose where they want the balls to be placed. 
Some of the skills I utilized were Embracing failure and Organization. As you saw up above I had a great idea of making the code smaller and effective to use. However the code I came up with did not work. Despite this I will try to fix it the next time I work on it. On top of this I also resorted back to the [documentation](https://brm.io/matter-js/docs/) and looked at [w3schoo](https://www.w3schools.com/js/default.asp)l for help in my code. The other skill was Organization because I had switched over to my IDE. Lately I have been using my IDE for a lot of my classwork and Homework. As a result I have organized all my folders and comment on my own code more often to make sure I know what is going on. 


[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)
