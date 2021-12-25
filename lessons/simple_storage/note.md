# Lesson 1: Learning Solidity by creating my first smart contract

View the smart contract's creation on the test (Rinkeby's) Etherscan: https://rinkeby.etherscan.io/tx/0xc62fa9fc80009e135fd7c1e737ebb940998111a7cd5b550d07605301f855a99a

Account info: https://rinkeby.etherscan.io/address/0x46d623a1ad45db58b215441c7cdc94d25bb39d55

Here are the different primitive types: int256, uint256, bool, string, address, byte32

You can also use the following data structures: lists, maps

People[] public people;
mapping(string => uint256) nameToNumber;

Types of visibility in solidity: Encapsulation exists in Solidity: public, external, internal, private
1. public: can be called by everybody including functions witin the contract
2. external: the function can only be called outside the contract which it was created
3. private: can only be view within the contract. This is the default.
4. internal:  can only be called inside the contract which it was created

EVM: Ethereum Virtual Machine

state change functions are called transactions

Two keywords that do not require you to make a state change / transaction
1. view
2. pure

Struct are ways to define a new object in solidity. E.g.
`

	struct People {
		uint256 favoriteNumber;
		string name;
	}

People public person = People({ favoriteNumber: 2, name: “John”});
