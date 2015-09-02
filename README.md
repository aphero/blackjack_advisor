## PURPOSE
Instruct user what their next move should be after being dealt their first Blackjack hand.

## Break it down
The program contains the following methods:
* validate() - Ensures that user input is a valid before continuing.
* convert(card) - Takes a card string and converts it to integer in order to make it usable for other methods and calculations.
* hard_soft_pair(card1, card2, dealer, st, hd, pr) - Takes all three cards and all three hashes and finds the value that the user is looking for.
* next_move(choice) - Takes the hash value returned from hard_soft_pair and converts it into a readable response to the input.

## The Flow
As the user puts in values, each card is validated to ensure no funny business is going on.  After each card has been validated, they are converted to integers so that the hand can be summed up and any face cards can be used to reference the hashes.  Then these values are used to pinpoint the value that the user is looking for in the hash table.  Lastly, the returned value is converted into a response that the user can clearly understand.  For example: "You want to Double if you can or Stay"
