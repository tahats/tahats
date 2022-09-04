from turtle import Turtle, left 
STARTING_POSITION = [[0,0],[-20,0],[-40,0]] 
MOVING_DISTANCE = 10
RIGHT = 0
LEFT = 180 
UP = 90 
DOWN = 270
class Snake:
  def _init_(self):
    self.segments = [] 
    self.create_snake() 
    self.head = self.segments[0] 
  def create_snake(self):
    for position in STARTING_POSITION:
    new_segment = Turtle()
    new_segment.shape("square")
    new_segment.color("white") 
    new_segment.pu() 
    new_segment.goto(position) 
    self.segments.append(new_segment) 
  def move(self):
    for segment_number in range(len(self.segments)-1,0,-1):
      new_x = self.segments[segment_number-1].xcor()
      new_y = self.segments[segment_number-1].ycor()
      self.segments[segment_number].goto(new_x,new_y) 
     self.head.fd(MOVING_DISTANCE)
   def right(self): 
    if self.head.heading() != LEFT:
      self.segments[0].setheading(RIGHT) 
   def left(self):
    if self.head.heading() != RIGHT:
      self.segments[0].setheading(LEFT)
   def up(self):
    if self.head.heading() != DOWN: 
      self.segments[0].setheading(UP) 
   def down(self):
    if self.head.heading() != UP: 
      self.segments[0].setheading(DOWN)
