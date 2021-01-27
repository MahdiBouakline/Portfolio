<!DOCTYPE html>

# Mahdi's Portfolio #

### Preview ###
This is my computer science portfolio. It's a collection of 10 modules that I enjoyed the most, a package of my knowledge and what I learned this quadmester. Almost all my modules are from Khan Academy, as I believe I understood them best. Enjoy!

<img id="khan" src="https://support.khanacademy.org/hc/user_images/bxdMcLh5-h7PkoXFEWUb2Q.png">


## My top 10 list: ##
  
Modules  | Ranking
------------- | -------------
JavaScript  |   <img id="JS" src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/6a/JavaScript-logo.png/480px-JavaScript-logo.png">
Coding Challenge  | 1
Introduction to JavaScript  | 2
Advanced JavaScript:Natural Simulations  | 3
Advanced Games and Vizualtions  | 4
Computer Science Principles: programming  | 5        
Introduction to HTML/CSS  | 6
The Internet  | 7
Digital Information  | 8
Online Data Security  | 9
Algorithms  | 10

## 1. Introduction to JavaScript ##
  
I will continue to use this module as it is what we use to animate. HTML and CSS are wonderful tools when designing a basic website, but JavaScript goes that extra step to turn a decent website into a terrific one. My favourite part of this module was learning to add text and pictures to the screen to truly bring everything together in a satisfying manner, and one that pleases the eye. 

<canvas id="myCanvas" width="600" height="400" style="border:1px solid #000000;">
  <script>
background(186, 145, 20); // wooden table
ellipse(200, 200, 350, 350); // plate
ellipse(200, 200, 300, 300); 

fill(135, 24, 24);//sausage
ellipse(200, 200, 30, 300);

//Colour
fill(245, 230, 24);
//Potatoe
ellipse(150, 100,60, 60); 

//Colour
stroke(71, 31, 30);
//cracker
rect(200, 250,60, 60); 

//Colour
fill(255, 0, 0);
//Pepperoni
ellipse(250, 100,60, 60); 

//Colour
fill(245, 245, 240);
//Napkin
triangle(100, 100,60, 60, 10, 100); 

//Colour
fill(206, 219, 90);
//Biscuit
ellipse(100, 200,90, 90); 

//Colour
stroke(183, 217, 31);
//New Dorito flavour
rect(270, 190,60, 60);  
</script>
</canvas>



## 2. Introduction to HTML/CSS ##
I will continue to use this module as it is the foundation of website design. Without HTML and CSS none of the effective websites we currently use would be accessible. My favourite part of this module was learning to create a webpage that serces a purpose from scratch. The challenges and projects were often intriguing and random. Coding a travel destination or a recipe was very satisfying when comparing where you started to the end product.
<canvas id="myCanvas2" width="600" height="400" style="border:1px solid #000000;">
  <script>
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>Mahdi Bouakline</title>
        <style>
        body{
            background-color: yellow;
            /*color: lightcoral;*/
            font-family: cursive;
        }
        .title{
            text-align: center;
            color:blue;
            
   }
        #dont{
            color:red;
            font-weight: bold;
            font-style: italic;
        }
        #list{
            color:black;
            float:left;
            border: outset crimson 2px;
            width:30%;
            margin-left:20px;
        }
        #hopper{
            position: absolute;
            width:50px;
            right: 25px;
        }
             #scrolldown{
            color:black;
            float:right;
            background-color:Green;
            width:55%;
            margin:auto;
            height:170px;
            overflow: auto;
            padding-left: 15px;
            padding-right:15px;
            margin-right:15px;
            text-indent: 25px;
            z-index:2;
        }
        #random-leaf{
            float:right;
            position:relative;
   text-align:left;
   padding-top:30px;
   width:100px;
   z-index: 5;
   /*margin-top:10px;*/
   }
   #welcome{
   position:absolute;
   top: 2px;
   left:5%;
   }
   </style>
   </head>
   <body>
   <img id="hopper" src="https://www.kasandbox.org/programming-images/avatars/leaf-green.png">
     
   <h1 class="title">Mahdi Bouakline</h1>
   <h2 class="title"> Cool Party </h2>
        
   <div id="list">
        
   <p class = "title">What to<span id="dont"> Get</span>:</p>
   <ul>
   <li>You</li>
   <li>Chips</li>
   <li>Cookies</li>
   <li>Your best friend</li>

            
   </ul> </div>
   <div id="scrolldown">
   <h3 class = "title">
   My Party?
   </h3>
   <p id="excuse">
   Super cool. whole computer science class is invited. 
   </p>
            
            
   </div>

   <a > <img id = "welcome" src="https://www.kasandbox.org/programming-images/avatars/duskpin-ultimate.png"></a>
        
        
 </body>
</html>
</script>
</canvas>

 
## 3. Advanced Games and Vizualtions ##
I will continue to use this module as it is essential to coding basic games and entertaining skits. This module helped me learn to create very fun mini-games, such as Tic-Tac-Toe and matching games. In terms of final product, this module was by a landslide my favourite of them all. It made me feel good about myself when I completed the games and saw what I was capable of. My favourite part of this module was learning to use loops and if statements to create those smaller games, and even incorporating characters into them. The challenges and projects were always a new game you could create and play afterwards.
<canvas id="myCanvas3" width="600" height="400" style="border:1px solid #000000;">
  <script>
//I used the numTries variable from free code camp, the idea to have a counter was from there. Some of the rnadom functions were from fcc
//Lining up tiles
var Tile = function(x, y, face) {
this.x = x;
this.y = y;
this.face = face;
this.width = 70;

};

//The tiles while they're face down
Tile.prototype.drawFaceDown = function() {
    fill(214, 247, 202);
strokeWeight(2);
rect(this.x, this.y, this.width, this.width, 10);
image(getImage('avatars/leaf-green'), this.x, this.y, this.width, this.width);
this.isFaceUp = false;
};

//Outputting rectangle and image
Tile.prototype.drawFaceUp = function() {
fill(214, 247, 202);
strokeWeight(2);
rect(this.x, this.y, this.width, this.width, 10);
image(this.face, this.x, this.y, this.width, this.width);
this.isFaceUp = true;
};

Tile.prototype.isUnderMouse = function(x, y) {
    return x >= this.x && x <= this.x + this.width  &&
y >= this.y && y <= this.y + this.width;
};

var NUM_COLS = 5;
var NUM_ROWS = 4;

// Declaring an array

var faces = [
getImage('avatars/leafers-seed'),
getImage('avatars/leafers-seedling'),
    getImage('avatars/leafers-sapling'),
getImage('avatars/leafers-tree'),
getImage('avatars/leafers-ultimate'),
getImage('avatars/marcimus'),
    getImage('avatars/mr-pants'),
getImage('avatars/mr-pink'),
getImage('avatars/old-spice-man'),
getImage('avatars/robot_female_1')
];

// An array with 2 and randomizing it

var possibleFaces = faces.slice(0);
var selected = [];
for (var i = 0; i < (NUM_COLS * NUM_ROWS) / 2; i++) {


var randomInd = floor(random(possibleFaces.length));
var face = possibleFaces[randomInd];

selected.push(face);
selected.push(face);

// Remove from array
possibleFaces.splice(randomInd, 1);
}

// Random array
selected.sort(function() {
return 0.5 - Math.random();
});

// Create the tiles
var tiles = [];
for (var i = 0; i < NUM_COLS; i++) {
for (var j = 0; j < NUM_ROWS; j++) {
tiles.push(new Tile(i * 78 + 10, j * 78 + 40, selected.pop()));
}
}

background(255, 255, 255);

// Now flip them
for (var i = 0; i < tiles.length; i++) {
tiles[i].drawFaceDown();
}

var flippedTiles = [];
var delayStartFC = null;
var numTries = 0;

//If statements to verify that they do or don't match
mouseClicked = function() {
for (var i = 0; i < tiles.length; i++) {
if (tiles[i].isUnderMouse(mouseX, mouseY)) {
if (flippedTiles.length < 2 && !tiles[i].isFaceUp) {
tiles[i].drawFaceUp();
flippedTiles.push(tiles[i]);
if (flippedTiles.length === 2) {
numTries++;
if (flippedTiles[0].face === flippedTiles[1].face) {
flippedTiles[0].isMatch = true;
flippedTiles[1].isMatch = true;
}
delayStartFC = frameCount;
loop();
}
}
}
}
//Outputting message if they are all found with the amount of tries declared with a variable called numTries
var
foundAllMatches = true;
for (var i = 0; i < tiles.length; i++) {
foundAllMatches = foundAllMatches && tiles[i].isMatch;
}
if (foundAllMatches) {
fill(0, 0, 0);
textSize(20);
text('It took you ' + numTries + ' tries!', 20, 375);
}
};

//Ending loop if there's no more unflipped tiles left
draw = function() {
if (delayStartFC && (frameCount - delayStartFC) > 30) {
for (var i = 0; i < tiles.length; i++) {
if (!tiles[i].isMatch) {
tiles[i].drawFaceDown();
}
}
flippedTiles = [];
delayStartFC = null;
noLoop();
}
};  
</script>
</canvas>


## 4. Advanced JS:Natural Simulations ##
I will continue to use this module as it is very commonly used in advanced games. All proper high budget games incorporate real life mechanics, such as physics. This module helped me learn to create advanced natural scenarios and reflect them onto a canvas. It taught me to create rainfall and motions such as bounce. In terms of final product, this module was not the best result, but it's purpose was the final goal. It taught me to take games to that next level and replicate functions in our universe and how to incorporate them. My favourite part of this module was learning to use older and new variables to update the position of every object and the random function to randomize their movement. 
<canvas id="myCanvas4" width="600" height="400" style="border:1px solid #000000;">
  <script>
//Used modules from free code camp
//radians instead of degrees as instructed by free code camp
angleMode = "radians";

//defining the properties of the flower
var Flower = function(){
    this.position = new PVector(width/2, height-100);
    this.mass = 40;
};

//displaying the Flower
Flower.prototype.display = function(){
    //four pedals
    fill(225, 255, 0);
    ellipse(this.position.x+13, this.position.y-89, 16, 16);
    ellipse(this.position.x, this.position.y-102, 16, 16);
    ellipse(this.position.x, this.position.y-76, 16, 16);
    ellipse(this.position.x-10, this.position.y-89, 16, 16);
    //center of flower
    fill(8, 8, 8);
    ellipse(this.position.x, this.position.y-89, 10, 10);
    //flower stem
    stroke(9, 235, 62);
    strokeWeight(4);
    line(this.position.x, this.position.y+100, this.position.x, this.position.y-65);
};

//defining particles
var Particle = function(position){
    this.acceleration = new PVector(0, 0.05);
    this.velocity = new PVector(random(-1, 1), random(-1, 0));
    this.position = position.get();
    this.timeToLive = 250;
};
Particle.prototype.run = function() {
    this.update();
    this.display();
};

//changing velocity and acceleration
Particle.prototype.update = function(){
    this.velocity.add(this.acceleration);
    this.position.add(this.velocity);
    //decreasing time to live by 2 so that it disappears around the time it reaches the ground
    this.lifeT -= 2;
};

//displaying particles
Particle.prototype.display = function() {
    noStroke();
    fill(156, 237, 255, this.timeToLive);
    ellipse(this.position.x, this.position.y, 12, 12);
};

//determining if particle is dead 
Particle.prototype.isDead = function() {
    if (this.timeToLive < 0) {
        return true;
    } else {
        return false;
    }
};
var Water = function(position){
    Particle.call(this, position);
};
Water.prototype = Object.create(Particle.prototype);
Water.constructor = Water;

//Rainfall
Water.prototype.display = function(){
    noStroke();
    fill(5, 26, 255);
    ellipse(this.position.x, this.position.y, 5, 5);
};

var ParticleSystem = function(position) {
    this.origin = position.get();
    this.particles = [];
};

//adding new particles
ParticleSystem.prototype.addParticle = function() {
    //always adding water praticles
    this.particles.push(new Water(this.origin));
};
ParticleSystem.prototype.run = function() {
    for (var i = this.particles.length-1; i >= 0; i--) {
            for (var i = this.particles.length-1; i >= 0; i--)    {
            var p = this.particles[i];
            p.run();
            //removing dead particles
            if (p.isDead()) {
                this.particles.splice(i, 1);
            }
        }
  }
        
};

//creating array of particleSystem
var particleSystem  = [];
//variable for the x value of the particle origin
var w = 25;
//adding new particle systems to the array
for (var i = 0; i < 4; i++){
        particleSystem.push(new ParticleSystem (new PVector(w, 0)));
        //increasing x value of origin
        w = w+100;
    }

//insect properties
var insect = function() {
    this.a = 0;
    this.angVelocity = 0;
    this.angle = new PVector();
    this.velocity = new PVector(random(-0.05, 0.05), random(-0.05, 0.05));
    this.amplitude = new PVector(random(20, width/2), random(20, width/2));
    this.position = new PVector(0, 0);
};

//oscillating the insects
insect.prototype.oscillate = function() {
    this.angle.add(this.velocity);
    this.position.set(
                sin(this.angle.x) * this.amplitude.x,
                sin(this.angle.y) * this.amplitude.y);
    var distance = this.position.mag();
    this.angVelocity += distance / 1000000;
    this.angVelocity = constrain(this.angVelocity, 0, 0.1);
    this.a += this.angVelocity;
};

//displaying the insects
insect.prototype.display = function() {
    pushMatrix();
    translate(width/2, height/2);
    stroke(20, 1, 1);
    strokeWeight(4);
    imageMode(CENTER);
    translate(this.position.x, this.position.y);
    rotate(this.a);
    //bee
    stroke(0, 0, 0);
    strokeWeight(2);
    fill(0, 0, 0);
    //head
    ellipse(-28, 0, 20, 20);
    fill(255, 255, 0);
    //body
    ellipse(0, 0, 48, 48);
    fill(0, 0, 0);
    popMatrix();
};

//new flower variable 
var flower = new Flower();

//declaring array for new insects
var bug = [];
//randomizing insects
for (var i = 0; i < 2; i++) {
    bug[i] = new insect(random(0.1, 2), random(width), random(height));
}

draw = function() {
    
   //sky
   background(56, 62, 64);
    
   //looping through array of particle systems 
   for (var i = 0; i < particleSystem.length; i++){
        particleSystem[i].addParticle();
        particleSystem[i].run();
        
   }
    
   //sun 
   fill(255, 247, 0);
    ellipse(279, 18, 158, 100);
    
   //clouds
    fill(87, 82, 82);
    noStroke();
    ellipse(66, 18, 158, 137);
    ellipse(181, 18, 100, 107);
    ellipse(351, 18, 158, 120);

   //dying tree
    fill(41, 29, 2);
    rect(0, 340, 150, 50);
    //grass
    fill(32, 74, 0);
    rect(0, 370, 400, 100);
    
   //dead bee
    stroke(0, 0, 0);
    strokeWeight(2);
    fill(0, 0, 0);
    //head
    ellipse(350, 380, 20, 20);
    fill(255, 255, 0);
    //body
    ellipse(380, 380, 48, 48);
    fill(0, 0, 0);
    
   //looping through all the bugs and displaying and oscillating them
    for (var i = 0; i < bug.length; i++){
        bug[i].display();
        bug[i].oscillate();
    }
    
   //displaying flower
    flower.display();
};

</script>
</canvas>


## 5. Computer Science Principles: programming ##
I will continue to use this module as it is essential to understanding programming and everything surrounding the subject. This module helped me understand the basics of coding, and how to use functions and more basic principles. It taught me what certain functions were used for. In terms of final product, this module didn't really have a physical one, but rather simply taught you it. The final goal was to teach the basics of coding and it fulfilled it successfully. It helped prepare me for what was to come. My favourite part of the module was taking the final tests at the end, and competing them to the quizzes at the beginning, it helped me realize how far I'd actually gotten and how much more I had to learn.   

  
## 6. Coding Challenge ##
This module was one of the more fun ones. I will continue to use the concept of this module, to take a basic code and splice it up. This code taught me to take something small with potential and turn it into a wonder. This project was the most enjoyable project of the course, it offered a small project with a partner, and was enjoyable team work. This project let you combine your ideasa, with that of your partner to create the best final product possible. The best part of this module was struggling to find something to add to it. I spent a long time on a call with jason tryng to figure out what we could change. Overll, this was really the only group project in the course, and it turned out to be very enjoyable.
  https://github.com/davidklimantovich/2DBlackHolePersonalChange

https://github.com/KaelanKM/Attraction-Repulsion-Refactoring-Kaelan


  
## 7. Computer Innovation & The Internet ##
I will continue to use this module as it helps me understand how the internet functions, and connects to our daily life. This module helped me understand the very small details of the usage, creation anf cunction of the internet in our society. It changed how I looked at technology and moern media, I looked at it through a different lense, one that knew how it all worked. My favourite part of this module the computer innovation, as it featured some of the best technology on the planet and explained how we'll use it, and continure to improve it, such as A.I..     



## 8. Digital Information & Algorithms ##
I will continue to use this module as it is the most often used in coding. This module helped me understand the true meaning of Algorithms, and how coding works to create the final product. It wen very in depth into what the code does when it is typed in, and how it works to produce a stunning final outcome. My favourite part of this module was learning bites aspect, it was something I'd never seen or been taught before, and it was crazy to understand how all these things came together. The content was a bit hard to understand at first, but when it sunk in, I realized what it meant and how it all worked.   


  
## 9. Online Data Security & Data Analysis & Security ##
I will continue to use this module as it is taught me how to keep my online information safe, and how it keeps it safe in the first place. This module taught me something we hear about often, but don't really get to see, and that is security. It taught me that many conventional things we do, don't actually keep you safe. Instead, it offered a substitution to that, and other ways to keep our private informaton safe.



## 10. TBD ##
TBD
