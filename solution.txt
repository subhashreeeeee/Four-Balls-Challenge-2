int xCircleOne, xCircleTwo, xCircleThree,  xCircleFour = 0;
final int UNIT_SPEED = 1;
final int WIDTH = 640;
final int HEIGHT = 362;
final float ONE_FIFTH_HEIGHT = (float)(double)HEIGHT/5;
final int DIAMETER = 10;

void settings() {
  size(WIDTH, HEIGHT);
}

void draw() {
  drawCircleOne();
  drawCircleTwo();
  drawCircleThree();
  drawCircleFour();
}

//the first circle is at 1/5th of total height from top and moves at a distance of 1
void drawCircleOne() {
  ellipse(xCircleOne, ONE_FIFTH_HEIGHT, DIAMETER, DIAMETER);
  xCircleOne += UNIT_SPEED;
}

void drawCircleTwo() {
  ellipse(xCircleTwo, 2 * ONE_FIFTH_HEIGHT, DIAMETER, DIAMETER);
  xCircleTwo += 2 * UNIT_SPEED;
}

void drawCircleThree() {
  ellipse(xCircleThree, 3 * ONE_FIFTH_HEIGHT, DIAMETER, DIAMETER);
  xCircleThree += 3 * UNIT_SPEED;
}

void drawCircleFour() {
  ellipse(xCircleFour, 4 * ONE_FIFTH_HEIGHT, DIAMETER, DIAMETER);
  xCircleFour += 4 * UNIT_SPEED;
}
