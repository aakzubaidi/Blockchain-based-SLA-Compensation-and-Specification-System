# Blockchain-based-SLA-Compensation-and-Specification-System
Hyperledger Fabric Blockchain-based SLA Specification and Compensation System


Prequisites: 

Assumptions


Settings
nvm use v8.15.0


-Run steps


First and before anything else, start from a clean setting: run this command
./byfn.sh down

composer card delete -c PeerAdmin@byfn-network-org1
composer card delete -c PeerAdmin@byfn-network-org2
composer card delete -c alice@sla-feasibility
composer card delete -c bob@sla-feasibility
composer card delete -c admin@sla-feasibility
composer card delete -c PeerAdmin@fabric-network

and then 
rm -fr $HOME/.composer

it also maybe useful to clear all docker images, containers, volumes releated to Hyperledger fabric or composer.

./byfn.sh up -o etcdraft
this will run 
