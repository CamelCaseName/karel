void walkTheLabyrinth(){
    while(!onBeeper()){
        if(frontIsClear()){
            moveForward();
        }
        else if(leftIsClear()){
            turnLeft();
            moveForward();
        }
        else if(rightIsClear()){
            turnRight();
            moveForward();
        }
        else{
            turnAround();
            moveForward();
        }
    }
}