Link to my Narative: https://editor.p5js.org/TWayneBlakemore/present/-MQ9Y5-8z

Code:

function setup() {
createCanvas(860, 800);
background(0);
}
function draw() {

  
//Bottom Left Square
fill(22, 166, 77);
square(0, 720, 200);
  
//Right Blue Square
fill(2, 144, 400);
square(620, 50,800);
  
  
//Left Purple Square
fill(255, 25, 255);
square(-500, 7,700);
  
//Upper Brown left Square 
fill(15, 40, 0);
square(0, 7, 120);
  
  
//Yellow Center Cube
fill(500, 245, 0);
square(250, 300, 320);
  
//Top White Cirlce
fill(500, 500, 500);
circle(410, 30, 390);
  
//Bottom Red Cirlce
fill(500, 0, 0);
circle(420, 800, 290);
  
}

I wanted to create something along the lines of Piet Mondrain. This piece is an abstract painting of shapes. I tried to recreate a similar feeling but while doing it through code. It was pretty fun to be completely honest. 

Link to my Interactive: https://editor.p5js.org/TWayneBlakemore/present/7RN7GFD-Y

Code:

let x = 200;
let y = 200;
let extraCanvas;

function setup() {
  createCanvas(400, 400);
  extraCanvas = createGraphics(400, 400);
  extraCanvas.clear();
  background(0);
}

function draw() {
  
  // No trails!
  background(0);
  x += random(-5, 5);
  y += random(-5, 5);
	
  // trails
  if (mouseIsPressed) {
    extraCanvas.fill(255, 150);
    extraCanvas.noStroke();
    extraCanvas.ellipse(mouseX, mouseY, 60, 60);
    let starX = random(width);
    let starY = random(height);
    extraCanvas.ellipse(starX, starY, 10, 10);
    //extraCanvas.ellipse(mouseX, mouseY, 60, 60);
  }
  
  image(extraCanvas, 0, 0);
    fill(255, 0, 0);
  stroke(255);
  rectMode(CENTER);
  rect(x, y, 20, 20); 
}

I did not have as much interest in this part of the project. I couldn't think of anything too creative. My link does not even seem to be working correctly, however the code alone does. What is suppose to happen is that there is a moving red square that you can't control but everytime the mouse click you are able to draw and it does not get on top of the red square. Also every time you click random dots are suppose to show up on the screen.

