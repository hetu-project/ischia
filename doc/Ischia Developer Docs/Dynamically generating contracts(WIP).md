# Dynamically generating contracts

### Introduction

On the Ischia platform, contracts can be generated dynamically by configuration (without writing code).

There are two main types of contracts: 

- the contract for the rules of the event points
    
    ![Untitled](Dynamically%20generating%20contracts/contract-rules.png)
    
    The project manager selects the event type in the Campaign through the Ischia Web Client，and Ischia automatically generates the corresponding rule contract，The user can access the rule contract through the router.
    

- the contract for the redemption points.
    
    ![Untitled](Dynamically%20generating%20contracts/contract-points.png)
    
    There are three main types of credit contracts. One is the contract provided by the platform, which simply counts user credits. The second is that the project manager calculates points according to the classification of different Campaign tasks; The third is mainly used with the reputation system