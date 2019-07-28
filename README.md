# Identity Management for elections, referenda and polls
A Proof Of Concept to implement a secure and reliable way to add citizens to Voters List

## What we're planning to build
We're planning to build a system that manages users/citizens in the electoral roll. Our solution aims to be more secure and transperant than the current system. We want to ensure deduplication and open accesiblilty. 

## How does it work?
Each block in the blockchain will contain one user's data. A smart contract will verify each block. The smart contract will have multiple functions. One pre-requisite to add the block will be the user's age. The smart contract will be responsible for checking the age. The smart contract will also have a model which will validate the user's documents using machine learning. It will check if the data(image) is tampered with and also with online databases. The user will also have to upload a recent photo of themselves. Other voters in the blockchain can verify this transaction. This measure is taken so that the same user doesn't register twice using different verification documents. We will build a face matching algorithm to ensure deduplication. 

## How can users get started with the project? (WIP)
Users will access a mobile application or a web-app to register to the electoral roll.

## What dataset(s) are we using? (WIP)
A dataset would be required to classify images as tampered or not. The dataset can be found [here](http://ifc.recod.ic.unicamp.br/fc.website/index.py?sec=5&source=post_page---------------------------). It contains 2 directories — one containing fake images and their corresponding masks and the other containing pristine images.  
[Reference link 1](https://towardsdatascience.com/image-forgery-detection-2ee6f1a65442)  
[Reference link 2](https://github.com/afsalashyana/FakeImageDetection)

## What technologies are we using?
1. Azure Blockchain
2. ReactNative or Flutter for cross-platform app development
3. Firebase for mobile backend
4. CNN for detecting tampered images
