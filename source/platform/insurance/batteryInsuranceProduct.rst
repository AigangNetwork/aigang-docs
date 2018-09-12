=================================
Android Battery Insurance Product
=================================

This insurance product is working example based on "Model Product for Phone Battery Insurance" data model.
Insurance product contains a description, terms and conditions and insurance product contract address.

Calculating Premium
^^^^^^^^^^^^^^^^^^^
Each user can calculate the specific premium for their device by following these steps:

1. Downloading Aigang App
2. Open the app and pair your device with the Aigang Platform.
3. In the Aigang Platform, press the button "Calculate Premium" button and enter your device ID.

Data from your device will be collected and sent to the premium calculator smart contract.
The premium calculator will validate the data and calculate the premium based on your device's data.

Insuring your device
^^^^^^^^^^^^^^^^^^^^
After calculating your premium you will be able to insure your device. 
You have to be logged in to your Metamask wallet and have the required amount on AIX tokens.
To insure your device just press "Insure" button in the policy window. 
Metamask will ask you to confirm your transaction.
After your transaction is confirmed, your policy status will be changed to "Paid" and your device
will be insured.


Insurance Product Smart Contract
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
All policies are stored in insurance product smart contract. 
Your policy ID is the key to getting your policy data from the smart contract.