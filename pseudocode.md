#Pseudocode for Washing Your Hands#

##INIT: Create variables for the program##
    1. **coldWater**
        *Offsets hotWater variable by one
        *Used to make sure hotWater does not reach a temperature too hot for placing hands in

**BEGIN**
 **INCREMENT** coldWater by 1
 **INCREMENT** hotWater by 2
 **IF** hotWater - coldWater === 1 **INPUT** hands
 **WHILE** Water is on **INCREMENT** soapOnHands by 2 pumps
 **IF** hotWater - coldWater = 1 && soapOnHands === 2 **THEN DECREMENT** soapOnHands
 **IF** soapOnHands === 0
**END**