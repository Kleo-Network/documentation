# Kleo SDK

Kleo's DATA DAO is open to building new projects from developers.


Integrating KLEO SDK is simple,
- The first step is to install the KLEO SDK!
```
npm i kleo-sdk
```

#### Accessing Personal Data Identity Information 

More about specific user. You can ask specific user questions such as, 

- What kind of movies has he seen?
- What sports is he interested in?
- Is the user tracking bitcoin and cryptocurrency prices?
- Is the user a web3 degen, share the NFTs he might have checked out?
- What videos has the user seen recently?

```
const userInfo = await Kleo.userInfo(
    user:'0xABV', 
    message:'has he searched about cricket world cup and betting games?')
```
Based on user settings and preferences it might respond in three possible answers,
- Share you the result
- Respond No 
- Share amount and user address

```
{"amount": 5, "address": 0x573aFF24788A7c28dE5E94C945e7b46a6f16f7C1}
```
Once you have made the transaction to the address, you need to call the same function again, 

```
const userInfo = await Kleo.userInfo(
    user:'0xABV', 
    message:'has he searched about cricket world cup and betting games?', 
    hash: 'transaction hash', 
    signature: 'signed message from the sender of transaction')

```

this time to get the right user data based on your questions. 


#### Accessing Data Pool Insights 

Kleo Data DAO Pools information of multiple users so there can be insights generated about multiple users, not only insights but Kleo can allow generation of powerful models on specific topic as well.

Here is how you can seek insights on multiple users' datasets'

```
const kleoSDK = await Kleo.pool(
    message: 'trading workflow of users',
    userLimit: 100
)
```
similarly, 
```
const kleoSDK = await Kleo.pool(
    message: 'shopping cart information',
    userLimit: 1000
)
```
The resulting will be json data of trading worklow of 100 users anonymized. 

