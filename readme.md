# ESTFORCE NFTs

## Workspace Structure

This workspace contains 3 directories:

1. **contracts:** Holds the contracts with increasing levels of complexity.
2. **scripts:** Contains four typescript files to deploy a contract. It is explained below.
3. **tests:** Contains one Solidity test file for 'Ballot' contract & one JS test file for 'Storage' contract.

## Scripts

The 'scripts' folder has four typescript files which help to deploy the 'Storage' contract using 'web3.js' and 'ethers.js' libraries.

**Deploying Other Contracts**

For the deployment of any other contract, just update the contract's name from 'Storage' to the desired contract and provide constructor arguments accordingly  
in the file `deploy_with_ethers.ts` or  `deploy_with_web3.ts`

## Tests

In the 'tests' folder there is a script containing Mocha-Chai unit tests for 'Storage' contract.

**Running Tests**

To run a script, right click on file name in the file explorer and click 'Run'. Remember, Solidity file must already be compiled.
Output from script will appear in remix terminal.

## Remix Module Support

Please note, require/import is supported in a limited manner for Remix supported modules.

**Supported Modules**

For now, modules supported by Remix are ethers, web3, swarmgw, chai, multihashes, remix and hardhat only for hardhat.ethers object/plugin.

**Unsupported Modules**

For unsupported modules, an error like this will be thrown: '<module_name> module require is not supported by Remix IDE' will be shown.