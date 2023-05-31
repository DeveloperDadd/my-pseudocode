# Pseudocode for Washing Your Hands #

## INIT: Create variables for the program ##
    1. ** coldWater **
        * Offsets hotWater variable by one
        * Used to make sure hotWater does not reach a temperature too hot for placing hands in
    2. ** hotWater **
        * Offsets coldWater variable by one
        * Used to kill bacteria on hands, and make sure water is at a comfortable level before placing hands in.
        * May require time to warm up
    3. ** soapOnHands **
        * Essential for making sure hands are clean
        * In the program can be incremented or decremented to indicate whether the program needs to keep running or not.
    4. ** paperTowel **
        * Required to dry hands off    
            

## Functionality ##

**Preparation Phase**

    FUNCTION setHotWater:
        IF hotWater < 2 
            THEN
                INCREMENT hotWater by 1 UNTIL hotWater === 2
                    END

    FUNCTION setColdWater:
        IF coldWater < 1
            THEN
                INCREMENT coldWater by 1 UNTIL coldWater === 1
                    END      

    FUNCTION putSoapOnHands
        IF hotWater === 2 && coldWater === 1
            INCREMENT soapOnHands by 1
                END

    FUNCTION rinseHands
        WHILE (hotWater === 2 && coldWater === 1 && soapOnHands === 1)
            INPUT hands into sink and DECREMENT soapOnHands
                END

    FUNCTION turnOffWater
        IF (soapOnHands === 0)
            DECREMENT hotWater until === 0
            DECREMENT coldWater until === 0
                END
    
    FUNCTION dryHands   
        GET paperTowel  
            THEN dry hands off
                END

**START: start the program**

    setHotwater()
    setColdWater()
    putSoapOnHands()
    rinseHands()
    turnOffWater()
    dryHands()
    
**END**