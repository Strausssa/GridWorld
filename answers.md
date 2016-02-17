# Part 1

## Set 1
1. The bug stays in a constant pattern moving around the grid. 
2. The direction that its head is pointing at is where it moves 
3. The bug rotates if it isn't moving
4. The bug leaves flowers behind
5. Rotates 90 degrees when the bug hits the wall
6. When a bug is going towards a rock, the bug will rotate 45 degrees and checks to see if there is a rock. If not, the bug then rotates another 45 degrees and goes forward toward the direction.  
7. The flower doesn't move
8. The flower changes color when a bug goes over it and turns darker as the bug goes further and further away. 
9. The Rocks can move but only if you use a certain method which is move and also change color
10. There can't be more than one figure in the grid because bugs and flowers can't.

### Exercises   
1. 0 : North
   45: North East  
   90: East  
   135: South East  
   180: South  
   225: South West  
   270: West
   315: North west
   360: North  
2. The moveTo method allows the bug to move in whatever direction but only if it is inside the bounds of the grid.
3.void setColor  
4. The bug is gone

# Part 2

## Set 2  

1. sideLength is the length of the box that BoxBug travels in  
2. steps tracks how many steps the boxbug moves so that it moves that specific amount  
3. It is called twice because it only turns the bug 45 degrees and in order to make a complete turn turn twice. 
4. Because the move function is inherited from the super class Bug.  
5. No you cannot change the square pattern as in there are no methods in which you change the variable sideLength so once the bug is constructed it cannot be changed!  
6. Obstacles in the path of the boxBug will cause it to change its path.  
7. Once you turn twice.  

### Exercises  
1.  CircleBug is different because it only turns once instead of twice which makes it move in a circular path instead of a square.Other than that it is very similiar.  

2. Spiral bug moves in a spiral and every single bug created is basically going to do what its name tell you.  
5. Check out the src code!    


# Part 3  

## Set 3  

1. loc1.getRow();  
2. false  
3.(3,5)    
4. South east  
5. You pass in the direction and the starting location, as the program translates the direction into coordinates, then it will execute and return the tile that has those transformations on the original.  

## Set 4    
1. Gets the count of objects in a grid by getting the size of the ArrayList for get occupied Location and get a count of the empty locations in a bounding grid by subtracting that number from the total number of grid spaces.  

2. the isValid() method  

3. The implementations would be found in the classes that use this interface  

4.No because ArrayLists are much more flexible for adjusting values in an array and can have adjusted values and different lengths based on the information passed to them.    

## Set 5 

1. Color, direction, location  
2. Default color is red and direction is north 
3. There are default methods for all actors and it wouldn't feasible to write all the methods within all the subclasses.
4. No and actor cannot be put onto a grid twice without removing itself and it can't remove itself twice. However it can be placed, remove itself and put back.
5. method turn() which will turn it 45 degrees, 2 turns is 90.  


## Set 6  
1. isValid() method to see if the place its moving to is on the grid.  
2.It checks to see if a space is empty or a flower which moves.  
3. isValid() and get() to check its moves  
4. getAdjacentLocation()  
5. getLocation()  
6. isValid() will return false and it will remove itself from the grid.  
7. It's not needed. 
8. Inherits the bugs color.  
9. No placing a flower is considered a move.  
10. flower.putSelfInGrid(gr, loc);  
11. 4 

## Group Questions:  

### 1.Specify  
a) It will move 1 space and jump over the rock or flower on the next jump.  
b) It will jump once and turn 90 degrees.  
c) Turn 90 degrees and resume jumping.
d) It will destroy the actor.  
e) Both destroyed.
f) No.    

### 2.Design  
a) Bug  
b) No 
c) Yes, the parameter should be grid
d) The act method should be overridden and  the constructor as well and canMove() and move()
e) A test for jumping such as canJump()
f) Creating a limited grid obstacle course for the bug involving other actors and obstacles.

### Code  
Done 

### Testing  
The jumper destroyed everything except the flowers and jumped 2 spots. Done.





