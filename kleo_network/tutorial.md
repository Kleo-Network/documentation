## Decryption and Dapp use cases 
This is split into two types of usecases, 
1. Accessing public profile of the user. 
2. Accessing private information of the user. 

Public information is built on social shares by the user using the kleo extension. These are randomly incentivezed and promoted in order to spread the word. This doesn't ensure ownership within data dao. 

There are two conditions required to be vetted to access the private information stored, 
1. They must be approved by Kleo data DAO. 
2. They must need the signature of the user they want to access information of, in order to decrypt the public key cryptography. 

 # Kleo 
Kleo uses public key cryptography to store your private / personal information, 
nobody without the signature can access your information. 

Although in order to protect user privacy we need to ensure that NO PII (Personally Identifiable Information) gets leaked about you. In order to ensure that, we run computations on stored data using LLM APIs on distributed TEE (Truster Executable Environment) with no manual intervention. Once the PII is removed then the entire history is encrypted with user's metamask signature and stored publicly on chain using IPFS. 
