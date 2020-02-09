# Beginner Friendly Lightning Network Guide

The Lightning Network (LN) was originally designed to make fast and cheap microtransactions on Bitcoin possible. The technology scales the transaction throughput of BTC to nearly infinite transactions per second since it’s a second layer solution. Fortunately the LN can be implemented on top of other blockchains as well. Decred is one of the first to do so.

This guide will show you how to use the LN on the Decred testnet. Testing is important to filter out the last bugs and it’s useful for anyone who wants to try out this new technology without risking real money.

If you have any questions, join the Decred chat rooms! https://chat.decred.org/

Steps to take:

### 1. You must have Decrediton installed

   - decred.org/wallets
   - If you already have Decrediton installed, check if you have the latest version (which is 1.5 at the time of writing)

### 2. Edit the config file to set "ln_enabled" to true

   - Make sure the Decrediton wallet is closed
   - Look for the config file in the Decrediton folder. The location of the config file location depends on OS: https://docs.decred.org/wallets/decrediton/decrediton-troubleshooting/#location-of-data-and-log-files
   - Open the config file with a text editor
   - Change the “ln_enabled” setting to true

### 3. Edit the config file to switch to testnet

   - In the same config file, switch “network” to “testnet”

### 4. Create a testnet wallet and let it sync (no SPV)

   - Start Decrediton and create (or restore) a full testnet wallet
   - While you wait for synchronization, go read some comics

### 5. Open your wallet and get free test DCR

   - https://faucet.decred.org will give free test DCR

### 6. Create a new DCRLND Wallet

   - If you did step 2 correctly, you can access the “Lightning Network” menu of your wallet to create a new LN Wallet
   - Decide if you want autopilot (not needed for this guide)
   - Click on “Start And Unlock LN Wallet”
   - Switch to the “Accounts” menu
   - Your new LN Account should show up

### 7. Send test DCR from the default to LN account

   - To use the LN Wallet you must have funds in it.
   - Go to the “Transactions” menu
   - In the “Send” tab, click the icon next to the “From” field
   - Select your new LN Account in the “To” field
   - Transfer a small amount to open a few channels
   - Go back to the “Lightning Network” menu
   - Wait for confirmationp
   - Congratulations, you are now ready to open channels ✅

### 8a. Open channels with LN Faucets on testnet

   - Go to the “Channels” tab in the “Lightning Network” menu
   - Go to one of the LN Faucets on testnet:
   - Example: https://testnet-dcrln-01.matheusd.com
   - Alternative: https://testnet-dcrln-01.davec.name
   - Scroll all the way down to the bottom
   - Copy the (node@ip:port) data shown above
   - Go back to your Decrediton wallet
   - Paste the data into the “Counterparty” field
   - Determine how big the channel should be
   - The “Push Amount” option allows you to send some DCR to the other party so you can receive them back as payments to test the channel. They are essentially a gift to the remote end to test all the functions
   - Click on “Open” and wait for confirmation
   - After confirmation, the pending channel will show as open
   - You can also view the channel status on the LN Faucet page

### 8b. Open channels with other LN nodes

   - Go to the “Channels” tab in the “Lightning Network” menu
   - Go to the testnet LN Map: https://ln-map-testnet.jamieholdstock.com
   - Choose a reachable node you want to connect with
   - (sometimes a node might show up as reachable, while the underlying dcrlnd node is not responding due to some issue)
   - Find the “Pubkey” and “Addresses” of the node
   - Go back to your Decrediton wallet
   - Enter Pubkey@Addresses into the “Counterparty” field
   - Determine how big the channel should be
   - The “Push Amount” option allows you to send some DCR to the other party so you can receive them back as payments to test the channel. They are essentially a gift to the remote end to test all the functions
   - Click on “Open” and wait for confirmation.
   - After confirmation, the pending channel will show as open
   - You can view all the open channels on the testnet LN Map

### 9. Close channels from your wallet

   - Go to the “Channels” tab in the “Lightning Network” menu
   - Click the cross in the right upper corner of an open channel
   - Click on “Confirm” and wait for confirmation

### 10a. How to create LN invoices

   - To receive value on the LN (within a channel or via hops), you must create an invoice. Every invoice can only be paid once.
   - Go to the “Invoices” tab in the “Lightning Network” menu
   - Add a fitting description
   - Request a value of maximum 0.00001 DCR
   - (maximum only applies to faucet invoices)
   - Click on the blue plus
   - Copy the invoice code

#### Optional: let the LN Faucet pay your invoice

When exchanging value with other LN nodes (step 8b), you simply send them the invoice code via chat. The other party can then pay the invoice (step 10b). If you are testing things out alone, use the LN Faucet to pay your invoices.

   - Go to one of the LN Faucets on testnet:
   - Example: https://testnet-dcrln-01.matheusd.com
   - Alternative: https://testnet-dcrln-01.davec.name
   - Scroll down to the “Pay Invoice” section
   - Paste your invoice code into the “Invoice code” field
   - Click on “Pay Invoice” ✅
   - The paid invoice should show up in the “Latest Invoices” section

#### Optional: generate invoices with the LN Faucet

When exchanging value with LN other nodes (step 8b), you will receive their invoice codes. You can then follow the steps below in 10b. If you are testing things out alone, use the LN Faucet to generate valid invoices.

   - Go to one of the LN Faucets on testnet:
   - Example: https://testnet-dcrln-01.matheusd.com
   - Alternative: https://testnet-dcrln-01.davec.name
   - Scroll down to the “Generate Invoice” section
   - Add a fitting description
   - Choose an invoice amount
   - Click on “Generate Invoice”
   - Copy the invoice code

### 10b. How to send LN payments

   - To send payments via the LN (within a channel or via hops), you must ask the other party for a valid invoice. Every invoice can only be paid once.
   - Go to the “Payments” tab in the “Lightning Network” menu
   - Paste an invoice code into the “Payment Request” field
   - The invoice details will automatically appear
   - Click on “Send” ✅
   - The payment should show up in the “Latest Payments” section

### Final notes

You should now have an idea about the basics of the Lightning Network. The user interface for Decrediton will likely change in the future, but the basic concepts will stay the same.

Thank you for helping us test the Decred Lightning Network and remember to send your test DCR back to the faucet after you’re done!
