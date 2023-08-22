Things used in the project:
   1. Solidity programming language.
   2. Ethereum.
   3. Remix IDE.


Architecture of the project:
   Global Variables:
   
      1. Owner: The real owner who deployed the contract.
      
      2. Start Time: The time when auction starts.
      
      3. End Time: The time when the auction ends.
      
      4. Highest Payable Bid: Highest person who is payable.
      
      5. Highest Bidder: The person who have bidded highest.
      
      6. Bid Increment: Increment bid by 1.
      
      7. Bidders: key value pair to keep track of bidders.
   Functions:
      1. Cancel Auction
      2. placeBid
      3. Finalize


How It works:
   1. There is an owner (the person selling the good or service), a start time, and an end time for the auction.
   2. If there is an emergency, the owner has the right to end the auction and cancel it.
   3. When someone calls the placeBid() function, they send ether. The sender address and sent value will then be registered in a mapping.
   4. Bidders are encouraged to offer the highest amount they are willing to pay because they are not restricted to the full amount but rather to the highest bid       that has come before it plus the increment. The specified amount will automatically be bid up in the contract.
   5. The selling price is determined by the highest payable bid, and the highest bidder is the auction winner.
   6. When the auction is over, the winning bidder receives the highest binding amount, and everyone else withdraws the amount they originally sent.


Output:
   1. truffle compile:
   
   ![image](https://user-images.githubusercontent.com/74295910/203910661-4e6b7d5f-480c-4291-82bb-33b8a7c72377.png)
   2. truffle migrate:
   
   ![image](https://user-images.githubusercontent.com/74295910/203910931-8eae4de0-d05a-4e8b-908e-dd535ab83c7b.png)
   3. ganache:
   ![image](https://user-images.githubusercontent.com/74295910/203911076-28f1616f-8cf4-4815-9055-8e474473f7d5.png)
   ![image](https://user-images.githubusercontent.com/74295910/203911163-fa0ce425-104e-420e-91a3-c9b66b104c31.png)
   ![image](https://user-images.githubusercontent.com/74295910/203911213-19bbc14a-238c-4abf-873f-3bddcf144008.png)
   ![image](https://user-images.githubusercontent.com/74295910/203911267-f5c7fd65-0930-4d44-886e-52d039be55df.png)
   ![image](https://user-images.githubusercontent.com/74295910/203911307-687171ac-fcf6-42d8-bb50-2586a615e482.png)




   
