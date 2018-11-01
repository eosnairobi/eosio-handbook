# Introduction

In this chapter, we shall explore what a Smart Contract is \(The definition as well as the structure of EOSIO Smart Contracts\), which shall then lead us to identifying what Ricardian Contracts are.

We shall then move on to writing our first basic smart contract \(the "Hello World"\) on EOS, as well as the ping-pong smart contract.

We shall then deploy these smart contracts onto our blockchain and interact with them.

Later in the chapter, we shall dissect through some slightly more complex Smart Contracts.

## What is a Smart Contract?

Borrowing from the definition of real-world contracts, we get to understand that a contract is an agreement that governs outcomes of actions, given a set of inputs.

_**Analogy 1.**_

An EOSIO Smart contract, thence, is _**software**_ that has been _**compiled**_ in a _**format that is acceptable, executable and retrievable**_ by EOS nodes. Just as the name suggests, EOSIO Smart contracts borrow from the structure of traditional contracts, only that in the case of EOS Smart Contracts, the _**actions, parameters, data structures and the code**_ that implements these aforementioned components are defined by the Smart Contract. All EOSIO Smart contracts are accompanied by Ricardian Contracts. We shall look at what Ricardian Contracts are shortly.

_**Analogy 2.**_

A smart contract in EOS could be described as a collection of actions \(steps that modify state\) and tables \(collections of state\).

They are analogous to applications, bound to identities \(each smart contract is associated to an account\), can be executed asynchronously and generate transactions.

## Ricardian Contracts Vs Smart Contracts

A Smart Contract is a machine readable set of instructions that organizes and controls the arrival of events, and the initiation of actions. A Ricardian Contract is a document that outlines the intentions and the actions that will be undertaken.

The **Ricardian Contract is the best effort to record the agreement**, and the **smart contract is the execution of said agreement.**

## Structure of an EOSIO Smart Contract

EOSIO Smart Contracts are composed of actions and data structures.

The data structures store the state of the blockchain, whereas the actions modify these particular states.

Actions accept parameters as laid out in the smart contract.



