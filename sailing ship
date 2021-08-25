var sea_bg, ship_up_down, ship_forw_back, sea, ship, edges ,shark
let playMode = 'sustain';
let sample;
function preload() {
  sea_bg = loadImage("sea.png")
  ship_up_down = loadAnimation("ship-1.png", "ship-2.png")
  ship_forw_back = loadAnimation("ship-3.png", "ship-4.png")
shark = loadAnimation("shark.png")
  soundFormats('mp3');
  sample = loadSound('sea.mp3');

}

function setup() {
  createCanvas(900, 800);
  

  sea = createSprite(850, 200, 400, 400)
  sea.addImage(sea_bg)
  sea.velocityX = -4
  ship = createSprite(200, 210, 10, 80)
  ship.addAnimation("float", ship_up_down)
  
  if (keyDown("space")) {
    ship.addAnimation("ship", ship_forw_back)
    
  }
  ship.scale = 0.4
  sea.scale = 0.4

}

function draw() {
sample.play()
  console.log(sea.x)

  if (sea.x < 0) {
    sea.x = 200;
  }
  background("white");
  edges = createEdgeSprites();
  drawSprites();

}