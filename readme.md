Liars Dice Rules
Each player is given a starting amount of dice.
A the beginning of each round each player rolls there dice, visible only to themselves
There are various rounds, each with whatever player who ends up losing giving up a dice.
The first turn of each round will make a bet (randomly decided for the first turn)
A bet consists of 2 aspects, a number and a corresponding dice to that number.
For example, a player could say 5 fours, meaning that believe there are 5 or more sixes in TOTAL on the table
After a player declares a bet, the turn moves to the next player in order, who is given 3 choices
1. The player can make another bet. There are two rules to this bet, if the player calls the same number as the previous bet (i.e the bet was 5 fours), they need to say a higher die face. So if something was bet like five fours,the player could bet five sixes, but not five twos. 
If the number is higher than the previous bet, any die face can be bet. If the call was 4 fours and the next player calls 5 fours, this move in legal.
2. The player can call BS, meaning they believe there are less than that many die on the field. When the player makes this call, all die are revealed and counted up.
It is important to note that 1's (unless bet first as discussed later), are wild, meaning they are to be counted as whatever the called die face.
CASE 1: There are strictly less than the number of die the player called on the table including 1's and the dice face (if ones aren't wild). This means the call was correct, and the player who made the previous bet loses a dice. A new round begins, with the player who called BS going first.
CASE 2: There are greater than or equal to the number of die the player called on the table. If this is the case, the call was incorrect and the player who made the call loses a dice. The player who called BS still goes first.
3. The player calls spot on. This means the player believes there are exacts as many die as the previous player called. So if the previous player called five fours, a spot on would require exactly five fours on the table.
CASE 1: If the player is correct, everyone besides the player loses a die, and the player begins the next round
CASE 2: If the player is incorrect, they lose a die.

Edge rules
1's are wild, meaning they are counted towards the total sum of dice at the end of a round
UNLESS the first bid is a 1, something like four ones.
Otherwise unless one is bid first, you cannot bid ones.



A gamestate for liars dice needs to include multiple things.
1. The overall game state. Some way to know whose turn it is, how many dice are on the table, what the dice are.
2. A way for a player to make a move either calling BS, spot on, or making there own call
For our purpose 0 will be BS, 1 will allow you to make a call, and 2 is a spot on call.
3. A way to resolve the move the player makes, and update the resolving move

