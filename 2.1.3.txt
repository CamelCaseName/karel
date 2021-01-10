void cleanTheTunnels(){
    while(frontIsClear()){
        cleantunnel();
    }
    cleantunnel();
}

void cleantunnel(){
    turnLeft();
    while(beeperAhead()){
        if(onBeeper()){
            pickBeeper();
        }
        moveForward();
    }
    if(onBeeper()){
        pickBeeper();
    }
    turnAround();
    while(frontIsClear()){
        moveForward();
    }
    turnLeft();
    if(frontIsClear()){
        moveForward();
    }
}