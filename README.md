# batamcoin-windows-v0.1
Test Mining Batamcoin (cryptonote) on Windows

1 } Create a Windows virtual Machine:
/Machine/Settings/Motherboard/Base Memory/4096MB
/Machine/Settings/Processor(s)/2
- with 2CPUs (virtual processor)
- 4GB of RAM
- 50GB of Dynamic Storage

2) Insert and run Guest Additions CD Image

3) Add paths to Shared Folders 
/Machine/Settings/Shared Folders/Add Share/
check Auto-mount
check Make Permanent

4) Download the batamcoin-windows folder into your Downloads folder

6) Run your Windows VM and the do the rest (Step 7 onwards) from within your VM:

7) Open command Promt and change directory to your local copy of batamcoin-windows
-  eg. cd Downloads\batamcoin-windows
-  ensure that you have the following:
    configs / batamcoin.conf
    lib     / batamcoind
            / miner
            / simplewallet
            / walletd
   And 3 batch files:
      - RunBatamcoind.exe
      - RunMiner.exe
      - RunSimplewallet.exe
      
8) Start a node
   Launch  RunBatamcoind.exe            
   A new Command Prompt will open
   Wait till you see the message:
   "You are now synchronized with the network. 
   You may now start simplewallet."
   
 9) Create a wallet address
   Launch  RunSimpleWallet.exe
   you see the following message:
      Nor 'generate-new-wallet' neither 'wallet-file' argument was specified.
      What do you want to do?
      [O]pen existing wallet, [G]enerate new wallet file, [I]mport wallet or [E]xit.

   type "G" and enter to generate new wallet file
   Sync from timestamp: 0
    Generated new wallet: BqUjgCKobtP1CjbfjPouAKZw8rR8GVyUJcrsRNicTgWbTp8W9T1ftSQKfy1zDhyDH5Bj2SmPMhFt7K5ut5KQQJGwBRoijer
    view key: d5f77d84098470ac39c47a3d8e6683b0bbaee3c9ea82383b68dd3f5e3c312701
    **********************************************************************

10) Copy and save both the new wallet address and view key

11) Go to windows explorer and right-click RunMiner.bat and select Edit
Replace the [Paste Your Wallet Address here] with your Wallet and save the file
  BqUjgCKobtP1CjbfjPouAKZw8rR8GVyUJcrsRNicTgWbTp8W9T1ftSQKfy1zDhyDH5Bj2SmPMhFt7K5ut5KQQJGwBRoijer 
  
12) Launch  RunSimpleWallet.exe
Happy mining New Batamcoin based on CryptoNote Technology based on Bytecoin (also similar to Monero) 
            
