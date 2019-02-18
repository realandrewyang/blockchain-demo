# blockchain-demo
An introductory blockchain demo for the UW Fintech Club

## Getting Started
Click on ```Clone or download``` to clone this repository or download a ZIP file.
You'll also need to download and install the [dependencies](#dependencies) for this project.

## Opening the Command Prompt
Once you've downloaded the files to a folder on your computer, you'll need to open up the command prompt on your computer.

On Windows, go to the Start Menu, search for ```cmd```, and you will find the Command Prompt.

On Mac, click ```Launchpad -> Other -> Terminal```

## Using the Command Prompt
In this demo, we will be using the command prompt extensively. Learning to use the command prompt is an integral part of being a programmer, but it can be a bit tricky to pick up. Here is a [cheat sheet](https://www.git-tower.com/blog/command-line-cheat-sheet/) that explains some commonly used commands to type into the command prompt.

First we need to enter the project folder (the place where you extracted the files from this repository). To do this in the command prompt, 
type ```cd PATH``` where PATH is the full path to the folder (for example, on my computer, the path would be ```C:\xampp\htdocs\blockchain-demo```).

Next, type ```geth --datadir=./chaindata init genesis.json``` and press ```ENTER``` to initialize the network.

Enter ```geth --datadir=./chaindata``` to display the blockchain data.

On Windows, enter ```geth attach ipc:\\.\pipe\geth.ipc``` to enter the Ethereum Javascript console.

On all other machines, enter ```geth attach```.

Now open up the Mist Wallet we downloaded earlier and create a new account with a username and password.

We are now ready to mine.

## Mining (READ THIS CAREFULLY)
For the purposes of this demo, I will show you how to start mining cryptocurrency. However, on this private network, the cryptocurrency you mine will not have any monetary value and will disappear as soon as you stop running the network.

In real life, bitcoin mining is done with specialized circuits designed to handle the massive number of calculations necessary to generate feasible returns.

**DO NOT ATTEMPT TO MINE CRYPTOCURRENCY ON A LAPTOP AS IT WILL OVERHEAT AND MAY SUFFER PERMANENT DAMAGE.**

To begin mining, we would enter ```miner.start(2);``` in the Javascript console.

To quickly stop mining, we could enter ```miner.stop();``` in the Javascript console.

## Dependencies
- [```Go Ethereum 1.8.22```](https://geth.ethereum.org/downloads/)
- [```Ethereum Mist Wallet 0.11.1```](https://github.com/ethereum/mist/releases)

Make sure to get the right version for your operating system (Windows, Mac OS, Linux, etc.)
