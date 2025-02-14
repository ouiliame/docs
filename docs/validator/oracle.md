# Oracle Feeder

Every validator is required to participate in the Oracle process, which involves periodically submitting a vote for the current exchange rate of Luna. Because these ballots are held very frequently, you will need to set up a program (called a feeder) to automatically submit votes. Failure to set one up will lead to downtime and missed votes, which past a certain threshold results in delegated stake getting [slashed](../dev/spec-oracle.md#slashing) and your validator temporarily jailed.

## Implementations

Below is a list of oracle feeder implementations you can choose from:

| Software                                                                | Developer                             | Runtime         |
| :---------------------------------------------------------------------- | :------------------------------------ | :-------------- |
| [`oracle-feeder`](https://github.com/terra-money/oracle-feeder)       | **Terra**                             | Node.js | Official reference implementation |
| [`terra_oracle_voter`](https://github.com/b-harvest/terra_oracle_voter) | [B-Harvest](https://bharvest.io/)     | Python          |  |
| [`terra-oracle`](https://github.com/node-a-team/terra-oracle)           | [Node A-Team](https://nodeateam.com/) | Go              |  |
