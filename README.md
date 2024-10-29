# Sample Hardhat Project

This project demonstrates a basic Hardhat use case. It comes with a sample contract, a test for that contract, and a Hardhat Ignition module that deploys that contract.

Try running some of the following tasks:

```shell

descargar proyecto
npm install
npx hardhat compile
npx hardhat ignition deploy ./ignition/modules/EcoStay.js --network ganache

en ecoStay.js 
/ Obtén el contrato desplegado (asegúrate de tener la dirección correcta)
  const contractAddress = "0x0F46F3EDc1b192095064E3EeeCecb9c1C0a36C3B"; // Cambia por la dirección real
  const EcoStay = await hre.ethers.getContractFactory("EcoStayTwo");
  const ecoStay = await EcoStay.attach(contractAddress);

npx hardhat help
npx hardhat test
REPORT_GAS=true npx hardhat test
npx hardhat node
npx hardhat ignition deploy ./ignition/modules/Lock.js
```
