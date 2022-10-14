# Wallet Selection Example from SmartPoker.io using Reach.sh on Algorand

## Demo
The repository is hosted on GitHub Pages at the following URL:
https://xarmian.github.io/smartpoker_wallet_example/index.html

## Explanation
This is an all-in-one example website for presenting a Wallet Selection dialog box using Vanilla Javascript with jQuery and Reach.sh.

This example is borrowed from the Cashier system for [SmartPoker.io](https://smartpoker.io), and demonstrates the following processes:
1. User selection of Wallet (i.e. Pera Wallet, Defly, WalletConnect, MyAlgo)
2. User selection of alternate node (AlgoNode vs. Algoexplorer)
3. Store/Restore data in Browser Local Storage, and restoration of app state on website reload

Once a Wallet has been connected, basic account information is displayed along with icons to allow a user to Disconnect the wallet, Refresh the display, and Copy the wallet address to the clipboard. Clicking the Disconnect button will clear the stored wallet data and return the user to the Wallet selection view.

This example is intended to be used by loading the index.html file directly in a modern web browser. This can be done by cloning the repository or downloading the index.html file and loading index.html locally, or by hosting the file on a web server.

## Disclaimer
This is a down-and-dirty example. As such there are no warranties or guarantees, and the code is messy.
