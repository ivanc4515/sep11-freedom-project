# Entry 3
##### 2/20/21

Since the last blog I have watched most of the [videos](https://www.youtube.com/watch?v=wB1pcXtEwIs&list=PLRqwX-V7Uu6akvoNKE4GAxf6ZeBYoJ4uh) I mentioned about [Matter.js](https://brm.io/matter-js/index.html). I started to work on a [test](https://repl.it/@IvanChiu/Matter-test#script.js) to see if I understand Matter.js properly. I tried to code some of the stuff in my IDE however I could not get it to work, so I continued to code on reple.it. I think that I have a pretty good idea about how Matter.js works now. In my test run of coding I made a simple world where blocks just spawn and are affected by different factors. For the most part the Engine takes care of the physics involved. For example the blocks will be affected by gravity and collide with other blocks. 

```
var engine = Engine.create();

var render = Render.create({
    element: document.body,
    engine: engine
});
```

Above, the code just shows the creation of the Engine and Render. The Engine runs all the physics in the world, while the render feeds the engine information of what is happening. Speaking about the World, in order for objects to appear in the world you need to make and add them in. Below you can see the creation of the blocks and adding them to the world. 

```
var objA = Bodies.rectangle(300, 200, 80, 80);
var objB = Bodies.circle(250, 30, 50);
var objC = Bodies.polygon(200, 100, 7, 45);
var groundA = Bodies.rectangle(400, 610, 810, 60, { 
  isStatic: true 
});
var groundB = Bodies.rectangle(150, 300, 400, 30, { 
  isStatic: true,
  angle: 3.33
});
var roof = Bodies.rectangle(400, 10, 810, 20, { 
  isStatic: true 
});

World.add(engine.world, [objA, objB, objC, groundA, groundB, roof, constraintA, constraintB],);
```

In the Engineering Design Process I’m on about a 2 and a 3. There are a lot of things I still need to learn on but I'm starting to see the pieces line up. I can see ways that I can use the things I learned and start to implement them into my final project. On top of this while I learn more about Matter.js I can see new ideas for my project. I don't want to change my idea completely but i think i will add things to my original game idea. 
<br>
The skills I learned I used were How to read and Embracing failure. I spent a lot of time reading the [documentation](https://brm.io/matter-js/docs/) and trying to understand the features I wanted to implement. For example the thing that I had trouble with was the Constraints. This was basically the connection between some of the blocks I made. The other skill Embracing failure was also related to the Constraints. I spent a lot of time trying to get the code to work. On top of that I tried to implement something called MouseConstraint. This would allow the user to interact with the block like picking them up and moving them around. However I could not find a way to make them work. This was unfortunate but I think if I put some more time into it I could get it to work. 


[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)
