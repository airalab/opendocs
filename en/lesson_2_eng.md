## Lesson 2: Distribute shares

> Difficulty: low.

**These Aira DAO Modules will be used:**

- `Shareholder token` ([abi](https://raw.githubusercontent.com/airalab/core/master/abi/TokenEmission.json))
- `Aira BuilderShareholder` ([abi](https://raw.githubusercontent.com/airalab/DAO-Factory/master/abi/BuilderShareholder.json))

### Lesson Description 

Some `shareholder tokens` were emitted when DAO was created. Now you need to distribute them to your team members.

You can do that in 2 different ways:

1. Send the tokens directly;
2. Call an `Aira BuilderShareholder` builder to create a `Shareholder` contract. When the `Sign` function is called, it will automatically withdraw a specified number of tokens from the `founder` to the `recipient` (specified during contract creation). 

The main difference is that, in the first case, the `recipient` becomes a shareholder automatically, without any approval. The second option requires explicit approval. The function `sign` is used for that.

> Notice: do not forget to call the `approve` function (see `Shareholder token` contract) to enable token withdrawal by `Shareholder` contract.

### Skill test 

> Complete this lesson and get 50 `ABT` tokens! 

**Instructions:**

- Allow the `Airalab learning center` address to withdraw 1 share of the `Shareholder token`. 
- Call the `Execute()` function from the `Lesson 2` contract.

