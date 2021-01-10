void hangTheLampions(){
    repeat(10){
        pickBeeper();
        turnLeft();
        while(frontIsClear()){
            moveForward();
        }
        dropBeeper();
        turnAround();
        while(frontIsClear()){
            moveForward();
        }
        turnLeft();
        if(frontIsClear()){
            moveForward();
        }
    }
}