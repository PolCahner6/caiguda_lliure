# caiguda_lliure
color c = color(2550);
float x = 0;
float y = 1;
float speedy=0;
float speedx=1;
void setup() {
  size(400,400);
}

void draw() {
  background(0);
  move();
  display();
}

void move() {
  x = x + speedx;
  speedy= speedy + 0.015;
  y = y + speedy;
  if (y > width) {
    y = 0;
  }
}

void display() {
  fill(c);
  rect(x,y,30,10);
}
