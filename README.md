Consignment Protocol
===

#### Data Verification in Decentralized Systems

Background
---

In many decentralized systems, users (or contributors) in the network contribute their computing resources in exchange for payments in tokens or cryptocurrencies. The biggest example of this is Bitcoin – where a group of miners achieve consensus by selecting the longest chain to follow. However, when solving real world problems, complex data structures and tasks are generated. Some of these projects include Golem and Gems, which tries to solve graphics rendering, machine learning, and even basic data entry, all in a decentralized manner.

The main issue with these decentralized applications is that there is a **strong incentive** for the participants in the network to cheat the system. Given a rendering task by a buyer in Golem, participants in Golem could cheat by generating random output that does not necessarily complete the task, but passes basic validation rules. By completing tasks more efficiently (cheating), the participant will be able to reap in more profits. This is obviously bad for the network as the buyers will lose trust in the the network's ability to do anything right.

One suggested method is to complete a random sub-task to verify that the whole computation or task is completed correctly. This brings a few issues:

1. Given a small enough task, there is little incentive to complete the sub-task to verify – the buyer could have just completed the task themselves.

2. Not all tasks are state-independent. Some tasks require execution from start to finish, and only the output is verifiable, not its intermediate results. An example of this is machine learning, where models have to be trained end-to-end without interruption.

3. If the threshold for verifying correctness is performing 50% of the task, there's little incentive to outsource the task to the decentralized network.

Solution
---

Consignment Protocol builds on multiple concepts:

1. Staking
2. Redundancy
3. Probabilistic correctness
