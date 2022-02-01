# Idea

## MVP

The contract outputs a single boolean for a function `isEthereumGreen()`

This value is determined by comparing 2 values: `costToCompensateUntilNow` and `sumCO2TokensBurned`

`sumCO2TokensBurned` starts at 0 and can be increased by sending funds to the contract. This also mints `N` NFT's where `N` is calculated by dividing the amount send by a stable value. This will also lead to the NFT being likely stable in price on secondary markets. This could be an interesting experiment on it's own. The funds are then converted to CO2 compensation tokens that are then burned. This might be batched to save on gas.

`costToCompensateUntilNow` is more complicated - it will either require an oracle or could be set by a DAO that is maybe consisting of people holding "I helped to make Etherum Green" NFTs or some independent group. It is calculated from 2 values `costsUntilTheMerge` and `anualCosts` multiplied by the years since the merge. To get a feel for `costsUntilTheMerge` you can [read this document](https://www.notion.so/Merge-4-Climate-9702d99a929e4f48af8fd90bfd205983) - but more research here is needed. But for the MVP some static values could be used that are upper bound estimates. But there should be the possibility to upgrade this to use different values or methods to get the values.

# After the MVP 

It would also be nice to see that people that helped making PoS possible (researchers, developers, testers, devops, auditors, stakers, ..) also get NFTs - but there the distribution is harder and maybe because of this outside the MVP. This also holds the opportunity to do an Airdrop to this group to get more traction and tick another buzzword for the bingo.

Also maybe interesting as a forcing function for some people could be a `leaderboard` which shows the ENS name of the persons holding most "I helped making Ethereum Green" NFTs. So you can still have the bragging rights so many search my having NFTs - without all the speculation (as the Price for these NFTs is stable)

Also it should provide a simple dapp where it outputs either something positive if `isEthereumGreen()` or something not so positive if the value is `false`. This dapp you can point people to when discussing the environmental impact of Ethereum and instead you have to argue - they are either just convinced or can open an issue for the project.

The MVP should be on and only include L1 - but to be more efficient it could move to an L2. Also at some point it should also include L2's impact on consumption. Maybe it should be a standard across chains that they provide a a IsThisProjectGreen contract.

# Timing / Launch

A nice time to launch this project could be the first block after "The Merge" - maybe just with the MVP at this point. The nice thing is this contract will not need to hold significant amounts of funds like some other contracts. So extensive security audtits would not even be cruitial - would still be nice to have more eyes on it - but maybe just for "I helped making Ethereum green" NFTs instead of having to pay the hefty prices for audits that you usually need for contracts that handle a lot of value.

# History

This idea was sparked by [this tweet](https://twitter.com/rabbyte/status/1488299042111115273) after [this initiative](https://www.notion.so/Merge-4-Climate-9702d99a929e4f48af8fd90bfd205983) which was relying on pure altruism did not really get the traction it needed. So maybe free riding this existing wave of NFTs could give it the traction it needs to return `true` for our core fun, help save some time in discussions, have a cleaner conciousness, and have a forcing function to make running Ethereum more energy efficient.

# License

CC0
