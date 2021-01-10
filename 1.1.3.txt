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

void defuseTwoBombs(){
    repeat(4){
        while(frontIsClear()){
            if(onBeeper()){
                pickBeeper();}
            moveForward();
        }
        turnLeft();
    }    
}