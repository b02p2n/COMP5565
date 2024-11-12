java c
COMP5565 Decentralized Apps Fundamentals and Development
Individual Assignment (10%)
[Deadline: 23:59:00 2nd November 2024 (Sat)]This is an individual assignment. You may use the course material and Internet resources to answer the questions. However, you should not post the questions online and ask for help.Discussion among your peers is encouraged; however, you must produce answers by yourself and in your own words. Any suspicion of plagiarism will be thoroughly investigated. Copying answers from GenAI tools into your assignment is a form. of plagiarism. Note that plagiarism is a serious offense. Both copiee and copier will receive 0 mark. Serious cases would be submitted to the Departmental for further disciplinary actions.
Question 1 – Modifying a Smart Contract (40 marks)Complete Lab 1 Task 6. Submit a completed file faucet.sol. Note that your solution must work in a real-world scenario, i.e., when any account tries to interact with the faucet in any order and for any number of times.
Submit a file called q1.sol.
Question 2 – Creating a Smart Contract (40 marks)
1.   Develop  a  Smart  Contract  that  enables  two  players,  each  having  an  EOA,  to play  a paper-scissor-stone game. When the contract is deployed, it has to be initiated with the two players’ EOA addresses. Before playing the game, the two players have to deposit 0.1 ETH to the contract. Only the two players can deposit ether to the contract. Each of them will trigger a function, play(), which accepts the choice of paper, scissor or stone, specified by the player. The play() function should determine who wins the game when it is called, provided that both players have called this function already. Only the two EOA addresses can trigger the play() function.The winner will receive 0.2 ETH from the contract account, which is the total deposit from both players. If there is a draw, each player will be refunded 0.08 ETH. After the game ends, the contract will be self-destructed and the account balance will be refunded to the EOA which deployed the contract.
You are allowed to develop other (internal) function(s) in your smart contract. Make sure the functions are having proper access control.At the beginning of the contract. Type the steps in details, in terms of comments, of how to deploy your contract, and how the game is set up and played by calling various functions of the contract.         [30pts]
Submit a file called q2-1.sol.
2.   In a near future, the SELFDESTRUCT opcode in the EVM (therefore, the selfdestruct() function in Solidity) will be deprecated. On a copy of your previous contract and make it work behave in an equivalent way while not relying on the selfdestruct() function.   [10pts]
Submit a file called q2-2.sol.
Question 3 – Improve a Faucet (20 marks)Take the front-end of the Holešky faucet you used during Lab  1,代 写COMP5565 Decentralized Apps Fundamentals and DevelopmentJava
代做程序编程语言 given in the attachment, and implement the following features using the ethers.js v6 library. Refer to the documentation at https://docs.ethers.org/v6/getting-started/. For this exercise, you will need to host the front-end on your localhost. A quick way to do so is to spawn a HTTP server using Node’s http-server package. Since we will later make use of NodeJS, why not prepare your environment now?
To install NodeJS, refer to https://nodejs.org/en/download/package-manager. On Windows, select prebuilt installer. Once installed, run the command:
npm install http-server -gto install the HTTP server. Finally, once placed on the directory that contains faucet.html, run the  server  using:  npx  http-server.  You  will  be  able  to  access  it  by  browsing  to http://127.0.0.1:8080(or see outputs from the command).
1.   Instead of copy-pasting the address into the text field, make the form. interact with the user wallet to select the proper account, populate the text field and disable the field to prevent  modifications   when  the   address  is  provisioned   from  the  wallet.  Add   a Connect/Disconnect button on the top right corner of the page to initiate the interaction with the wallet, or disconnect the wallet and revert back to manual input.            [10pts]
2.   When  an  address  is  input manually,  there are  opportunity  for making  mistakes.  If undetected, funds could reach a wrong address and become unrecoverable. Fortunately, Ethereum  addresses  often  come  with  an integrated  checksum. While  an  address  is approximately a hash of a public key with the result encoded in hexadecimal (which is case-insensitive), Ethereum checksumed addresses encode an extra checksum in the
letter case. For instance, this is an address without checksum:
0xc361fc33b99f88612257ac8cc2d852a5cee0e217
and this is the corresponding checksumed address:
0xc361Fc33b99F88612257ac8cC2d852A5CEe0E217
Implement a checksum verification of the supplied address and prevent the form. from being submitted if the checksum is invalid.                     [10pts]
Note that you will not have the backend to make the faucet work. Therefore, calls to the backend will show the error “Error: Unexpected end of JSON input”, which is normal.
Submit a file called q3.sol.
Submission
The deadline of this assignment is 23:59:00 2nd November 2024 (Sat). No late submission is allowed.
1.   Compress all files q1.sol, q2-1.sol, q2-2.sol and q3.sol into a single ZIP file
2.  Name this ZIP file as as Assignment__. E.g., Assignment_ 12345678d_CHANTaiMan
3.   Submit the file to the “Assignment” entry under “Assessments” in Blackboard.
Any wrong file naming and submission will receive 0 mark for the whole assignment. You have the obligation to check the correctness of your submission.

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
