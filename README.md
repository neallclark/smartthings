# smartthings
Smartthings scripts

The front of my house has 2 doors, 1 into a porch area and then a second into the hall.
Based on the sequence of doors opening and closing we can determine if someone is entering or leaving the house.

To use this script you should also add some virtual switches (I use the "simulated switch" device). You can then use 
these simulated switches in other smartapps to trigger various events.

The virtual switches cover the following events -
1. Someone is entering the house now (i.e. entered the porch from outside)
2. Someone is leaving the house now (i.e. entered the porch from inside)
3. Someone left (i.e. went through the porch from inside and shut all the doors behind them)
4. Someone entered (i.e. went through the porch from outside and shut all the doors behind them)

If all the doors are closed for one minute and the state is stuck at "someone is entering" or "someone is leaving",
then the states are reset one minute after all the doors are closed. One example would be when answering the door 
to take a delivery.
