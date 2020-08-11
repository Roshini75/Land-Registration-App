# Land-Registration-App
Land Registry Application

Land Registry Application using blockchain can build trust and transparency for Citizens while making the entire system more efficient. It provides security and verification through cryptographic proofs. In many countries land registries are not trusted or transparent if they exist at all in, 2017 the World Bank release the study stating that more than 70% of the global population lacks the legal claim to their land and 1/3 of countries do not digitally track property ownership Studies have resulted in increased uncertainty and friction in the marketplace that can often put a strain on governmental resources, especially in Judicial Systems for example in India, two-thirds of the legal dispute are related to land claims.
 
So keeping all these drawbacks of the present land registration in mind, I came with the idea of the land registry using secure blockchain architecture. This helps us to store the property records hashed and digitally signed. By doing this we can keep the registration process secure and trustworthy. So, we get the unique transaction details when one registers the land on his name or one transfers his existing land to the other person. So, first, we should develop a web app with all the features mentioned above in it and then integrate with the blockchain architecture.
 
To register the land, a citizen needs
1.	A suitable device(Desktop/PC/Tablet/Mobile)
2.	An Internet connection with at least 256kbps per second
3.	In PC/Laptop, any of the modern browser
 
For the guarantee of the application’s security and fault-tolerance, the application will be built on a blockchain architecture where all the transactions are verified and validated by the participants on the network. By using the blockchain the authenticity of the property records will be secured. This application provides advantaged such as trusted data storage, prevents tampering with a history log.
 
Land registry app has the following feature:
•	Helps to prevent the fraudulent transactions of property
•	Authentication using the registration details
•	The administrator can extract the property records with the hash value.
 
Increasing scams in the real estate have given the drive to make the land registration process digital where the property records are hashed and digitally signed.




In this project we have implemented the  following things
1)	We have hashed the land property transaction.
2)	We have hashed the land transaction from one user to another.
BLOCK CHAIN IMPLEMENTATION
Setup the environment to generate a Blockchain on Komodo platform. 
Step1: Download the executable files to your Windows computer and place the files in a new folder on the Desktop called Komodo. 
 
Step2: Create komodo.conf file in the below path C:\Users\tadir\AppData\Roaming\komodo
 

Step3: komodo.conf contains the following information. 
rpcuser=roshinitadi
rpcpassword=Rosh@1996
daemon=1
rpcallowip=127.0.0.1
rpcbind=127.0.0.1
server=1
txindex=1
maxconnections=1 

Step4: Create directory for Zcash Parameters. C:\Users\tadir\AppData\Roaming\ZcashParams  
 
 Step5: Run Smart Chain Software \Desktop\kmd\komodod.exe 
 Step6: Verify syncing process \Desktop\kmd\komodo-cli getinfo 
Create an address, wallet and add funds to the same.  Initializing the blockchain 
 komodod -regtest -ac_name=VCOIN -ac_supply=10000 & 
  
Displaying details of the chain generated. 
 Komodo-cli -regtest -ac_name=VCOIN getinfo 
  
 
 

Generating  blocks through cmd 
 Komodo-cli -regtest -ac_name=VCOIN generate 5 
 
  
Displaying details of the 1st block using blockhash. 
 Komodo-cli -regtest -ac_name=VCOIN getblock 040cf49c94db9e9b3f448b315d80f9578018b4164fe061f62a5138dbc6b0dc43
 

Test coins are now added to the block 
Komodo-cli -regtest -ac_name=VCOIN getinfo
 
Send a transaction between wallets on the Blockchain. 
Generate new address to demonstrate transaction between blocks 
Komodo-cli -regtest -ac_name=VCOIN getnewaddress 
RWtJrT4Gr4yrAX2WKrDqNkrVShfkNBXaoq
 
Coin info before transaction
Komodo-cli -regtest -ac_name=VCOIN getinfo
 
Now send the coins to the address RWtJrT4Gr4yrAX2WKrDqNkrVShfkNBXaoq
Komodo-cli -regtest -ac_name=VCOIN sendtoaddress RWtJrT4Gr4yrAX2WKrDqNkrVShfkNBXaoq 10
Hash 2939570d6edcfab720e369a89ad60cb7f9ae0b4527abd3f4b536102bb437e988
 

Coin info after transaction
Komodo-cli -regtest -ac_name=VCOIN getinfo – after deduction
 



Land Register Application 
Home screen

Available lands screen
 

Available users

Generated Hash after the land transaction to user
 


Generated Hash after the land transaction from a user to another user
 
Refer the documentation.dox and Readme.docx for more information
