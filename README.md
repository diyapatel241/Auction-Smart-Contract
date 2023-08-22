# Block-Chain-Technology
Things used in the project:

Solidity programming language.

Ethereum.

Remix IDE.

Architecture of the project: Global Variables:


  1. Owner: The real owner who deployed the contract.
  
  2. Start Time: The time when auction starts.
  
  3. End Time: The time when the auction ends.
  
  4. Highest Payable Bid: Highest person who is payable.
  
  5. Highest Bidder: The person who have bidded highest.
  
  6. Bid Increment: Increment bid by 1.
  
  7. Bidders: key value pair to keep track of bidders.

  8. Functions: 1. Cancel Auction 2. placeBid 3. Finalize

How It works:

There is an owner (the person selling the good or service), a start time, and an end time for the auction.
If there is an emergency, the owner has the right to end the auction and cancel it.
When someone calls the placeBid() function, they send ether. The sender address and sent value will then be registered in a mapping.
Bidders are encouraged to offer the highest amount they are willing to pay because they are not restricted to the full amount but rather to the highest bid that has come before it plus the increment. The specified amount will automatically be bid up in the contract.
The selling price is determined by the highest payable bid, and the highest bidder is the auction winner.
When the auction is over, the winning bidder receives the highest binding amount, and everyone else withdraws the amount they originally sent.
