# Wallet Selection/Connect Example using Reach.sh on Algorand

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

This example is intended to be used by loading the index.html file directly in a modern web browser. This can be done by cloning the repository and loading index.html locally, or by hosting the folder on a web server.

## Technical Details
In order to use with Pera Wallet's native connector, browserify and esmify were used to create a bundle of the @perawallet/connect library. While the Reach (@reach-sh/stdlib) library does not require this, it is included in the bundle for simplicity. This bundle, named `bundle.js` is created as follows, and included using `<script>` tags:

```npm install -g browserify
npm install --save-dev esmify
npm install @reach-sh/stdlib @perawallet/connect
browserify -p esmify -r @perawallet/connect -r @reach-sh/stdlib > bundle.js```

The example also uses jQuery/jQuery-UI and Font Awesome, which are loaded from CDNs.

## Disclaimer
This is a down-and-dirty example. As such there are no warranties or guarantees, and the code is messy.
