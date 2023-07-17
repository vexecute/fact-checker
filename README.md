# Fact-checker

**Created UI using typecript and reactjs for our hackathon project.**
<br>

### Problem Statement

The proliferation of fake news has become a significant challenge in today's digital age, leading
to widespread misinformation, erosion of trust, and negative societal impacts. Traditional
centralized fact-checking systems are often slow, centralized, and susceptible to biases and
manipulation, hindering their effectiveness in combating the spread of fake news. To address
this problem, we aim to develop a decentralized application (DApp) that leverages the power of
blockchain and distributed consensus mechanisms to create a reliable, transparent, and
community-driven platform for verifying the authenticity of news articles. The DApp will
empower users to independently and efficiently validate news sources, ensuring the
dissemination of accurate information and fostering a more informed and trustworthy media
landscape.
<br>

### Solution
* We are leveraging ICP's low gas cost and high transaction throughput to solve this issue
* The users are required to deposit a fixed amount in ckbtc (to create a request) and these are distributed to the votes who voted for the majority. Thus incentivising both requesters and votes to be behave honestly
* Each user can create a request passing the source of the news and their description . This will be voted by randomly selected group of users and the opinion of the majority is considered as final.

<br>

### Procedure
* **Phase 1** - The requester (user who wants request for a source to be verified ) calls the createMarket function with relevant links and description . The user also deposits a fixed amount (current 0.0001 ckbtc) .
* **Phase 2** - 
Voter :- A user can register as voter in the platform . Voter will also be required to maintain a fixed balance in the contract to right spams.
* **Phase 3** - The voters will be randomly selected and they will vote on whether the news is - **TRUE, FAKE or Undetermined**.
* **Phase 4** - The choice of the majority is considered as final. Those who voted for the majority are incentivised by the deposit of the requester



