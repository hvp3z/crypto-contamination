Crypto contamination is a Dapp game based on the tutorial crypto-zombies (https://cryptozombies.io/), by Loom Network.

Reminders concerning Dapps :
GENERAL TIPS
Important in DAPP learning : IMMUTABILITY OF a contract

When you put your contract “online” => you CAN’T FIX IT anymore / Nor make it evolve.

Never hard-code a contract’s adress

Application you create MUST inherit from Ownable, a contract made by https://openzeppelin.org/.

It allows you to have some security injected in your project, like “Only me can access this function” and shit. Check OpenZeppelin, that’s a mandatory point for developping DAPPS.
ABOUT GAZ

Because running functions costs real money for your users, code optimization is much more important in Ethereum than in other programming languages. => OPTIMIZE IT

To counter that : Dapps consuming resources => sidechains
               Dapps tiny consuming resources => Etherum mainnet

IN STRUCTS : Optimized gaz consuming : You'll want to cluster identical data types together ex int, int32, int32 instead of int32, int, int32
Careful, default uint is = 256 bits uint

One of the more expensive operations in Solidity is using storage — particularly writes. > Thousands of nodes across the world need to store that data on their hard drives, and this amount of data keeps growing over time as the blockchain grows

So use Memory as much as you can boi

Storage the less the better, iterating through cost money (gas) to your user
