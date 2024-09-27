java c
DSCI 216: Stochastic Computing
Written Exam #1
Section I: Events and Probabilities

Fig 1. Rolling a 4 on a D4
A four sided die (D4), shaped like a pyramid (or tetrahedron), has 4 flat surfaces opposite four corner points. A number (1, 2, 3, or 4) appears close to the edge of each flat surface. When rolled, the D4 comes to rest on one of its flat surfaces. The outcome of the roll is the number associated with the flat surface onto which the D4 comes to rest. An example D4 roll resulting in a 4 is depicted in Figure 4.
1. Write out the dense sigma-algebra for events concerning rolling a D4 (10 points)
2. For the dense sigma-algebra, not including the empty set ∅ or its negation, event " = {1,2,3,4}, if you were playing a guessing game involving the roll of a D4, what is an example of the easiest event to guess (if there is more than one, pick one)? Describe what makes it the easiest? (10 points)
3. What is an example of the hardest event to guess (if there is more than one, pick one)? Describe what makes it the hardest? (10 points)
Section I: Reliability

Plagued by intermittent issues during your cell phone contract, armed with the manufacturers specification of major components, you decide to disassemble your phone, trace the electrical connections and build a reliability model to determine which component has the biggest influence on the phone’s reliability.
You find your phone has four major subsystems

The cell phone’s antenna uses current from the battery to communicate by sending and detect electromagnetic signal energy in the air. The cell phone’s liquid crystal display (LCD) screen uses voltage from the battery to light it’s pixels. The camera uses voltage from the battery to power it’s motors to focus it’s lenses and operate its image capture circuits. The antenna, LCD screen, and camera do not depend on one another.
4. Draw a flow diagram depicting the dependencies among the battery, antenna, LCD screen, and camera. (5 points).
5. The battery has a failure rate of 5%, the antenna has a failure rate of 10%, the LCD screen has a failure rate of 15%, and the camera has a failure rate of 20%. What is the reliability for the system? Show your work. (15 points)
6. Which component has the largest influence on system operation? Explain using numerical examples and show all of your work. (10 points)
Section III: Random Vectors, Conditional Probabilities, and belief
A casino enlisted your help in the design of a new game entitled “cool coins” that involves flipping two coins whose outcomes are measured by random variables Coin1 and Coin2. The coins are flipped in order and their heads/tails outcomes are recorded. The challenge of the game is that the coins are biased and the player does not know the bias ahead of time. Your task is to analyze the game’s probabilities. Suppose you have observed the foll代 写DSCI 216: Stochastic Computing Written Exam #1Matlab
代做程序编程语言owing sequence of flips of (Coin1, Coin2) where h=heads and t=tails outcomes. For example (h,t) means Coin1=heads and Coin2= tails. The coins are independent.
(h, t) (h, t) (h, h) (h, h) (t, t) (t, h) (h, t) (h, t) (t, h) (h, t)
(h, t) (t, h) (h, t) (t, t) (h, t) (h, t) (h, t) (h, h) (h, t) (h, t)
7. What is the probability P(Coin1)? What is probability P(Coin2)? Show all of your work (10 points)
8. A new game begins, the first coin is flipped, and you observe “tails.” Using the historical data above and your observation that the newly flipped 1st coin had an outcome of “tails”, compute the probability for both outcomes (h and t) for coin 2 (10 points)
Modeling
A simulation for a simple game of chance involving a fair tetrahedron or 4-sided die has been specified via the following MATLAB (pseudo) code…NUM_TRIALS=-1;PLAYER_DATA= 1;HOUSE_DATA= 2;INITIAL_WALLET= 5000;playerWager= -1;houseWager= -1;houseWallet= INITIAL_WALLET;playerWallet= INITIAL_WALLET;trialNums= [ 2, 10, 500, 5000, 10000, 50000];NUM_EXPERIMENTS= length(trialNums);playerWagers= [ 1 ];houseWagers= [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];NUM_PWAGERS= length(playerWagers);NUM_WWAGERS= length(houseWagers);stickWeights= [ 10, 10, 10, 10];stickNames= {‘one’, ‘two’,’three’,’four’};playerGuess=’one’;data= zeros(1,NUM_EXPERIMENTS,2);for e=1:1:NUM_EXPERIMENTSNUM_TRIALS= trialNums(e);for p=1:1:NUM_PWAGERSfor h=1:1:NUM_HWAGERSplayerWager= playerWagers(p);houseWager= houseWagers(h);playerWallet= INITIAL_WALLET;houseWallet= INITIIAL_WALLET;for i=1:1:NUM_TRIALSif ( wager(playerGuess, stickWeights, stickNames) )playerWallet= playerWallet + houseWager;houseWallet= houseWallet – houseWager;elseplayerWallet= playerWallet – playerWager;houseWallet= houseWallet + playerWager;endenddata(1,e,PLAYER_DATA)= playerWallet;data(1,e,HOUSE_DATA)= houseWallet;endendendplotData(data);
9. In the experiment involving the tetrahedron, for what experimental parameterization will the player and house typically break event?
Explain why? (10 points)
10. Why is or isn’t it a good idea to run the experiment for 2, 10, or 500 trials?                 (10 points)
Strategies for Complex Probabilities
Clark Dining Commons has begun a Food Truck business, Cougar Eats! Because pantry space is small, a limited inventory of single serving food items is kept on the truck. Inventory covers the major food groups, namely a protein, a starch, a vegetable, and a beverage. To create a meal, a single serving is removed from the pantry from each category , boxed, and sold to the customer.

11. Given the pantry below how many different types of meal boxes is Cougar Eats able offer? (10 points)
Show all of your work

12. What is the probability of selecting a seafood dinner, that is a dinner that includes seafood? Show all of your work. (10 points)







         
加QQ：99515681  WX：codinghelp
