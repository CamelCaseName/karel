void tileTheFloor(){
    repeat(100){
        if(!onBeeper()){
            dropBeeper();
        }
        if(frontIsClear() && !beeperAhead()){
            moveForward();
        }
        else{
            turnLeft();
            moveForward();
        }
    }
}