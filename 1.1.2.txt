void defuseOneBomb(){
    while(!onBeeper()){
        moveForward();
    }
    pickBeeper();
    turnLeft();
    while(frontIsClear()){
        moveForward();
    }
    turnAround();
}