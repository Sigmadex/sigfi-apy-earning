<img src="https://user-images.githubusercontent.com/33762147/155625647-55c69f06-e0ea-44a8-a425-7aa086c329c5.png" style="border-radius:50%;width:72px;">

# Smart Contracts for SigmaFi Liberty Pool

## Summary

This application works in conjunction with an APY NFT and locks up SDEX or SDEX LP tokens for a user-selected period of time. As time elapses the smart contract will mint sSDEX tokens on a daily basis relative to the APY NFT attached and value of SDEX or SDEX LP compounded with their initial principal. After the timeframe has exceeded the selected period, the user will be allowed to withdraw their SDEX or SDEX LP tokens plus additional rewards with no penalty. If they choose to exit the position early, they will forfeit half of their entire principal. Minted rewards can be withdrawn with no penalties at any time however, doing so will prevent the initial principal from compounding.

**Distribution of penalized assets will be handled in 2 different ways:**
* SDEX will be forwarded to a multi-sig contract for removal of token circulation
* SDEX LP will be forwarded to `0x0000000000000000000000000000000000000000`

## Reward Rates

<div align="center">

|type|rate|
|----|----|
|SDEX|APY from NFT|
|SDEX LP|APY from NFT + LP Bonus|
  
</div>

## Penalty Rates

<div align="center">

|type|rate|
|----|----|
|SDEX|50% + NFT forefeit|
|SDEX LP|25%|
  
</div>
