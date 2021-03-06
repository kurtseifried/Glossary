```mermaid
graph LR
BlockchainArchitecture(BlockchainArchitecture)
BeaconChain -->|receives transactions from|ShardChain[Shard Chain]
BeaconChain -->|sends transactions to|MainChain[Main Chain]
Block -->|entered into|BeaconChain[Beacon Chain]
Block -->|entered into|Blockchain[Blockchain]
Block -->|entered into|MainChain[Main Chain]
Block -->|entered into|ShardChain[Shard Chain]
BlockExplorer -->|views transactions in|BeaconChain[Beacon Chain]
BlockExplorer -->|views transactions in|Blockchain[Blockchain]
BlockExplorer -->|views transactions in|MainChain[Main Chain]
BlockExplorer -->|views transactions in|ShardChain[Shard Chain]
BlockExplorer -->|views transactions in|Transaction[Transaction]
Blockchain -->|uses a|Consensus[Consensus]
BlockchainNetwork -->|can|HardFork[Hard Fork]
BlockchainNetwork -->|can|SoftFork[Soft Fork]
Consensus -->|can be|ProofofAuthorityPoA[Proof of Authority PoA]
Consensus -->|can be|ProofofStakePoS[Proof of Stake PoS]
Consensus -->|can be|ProofofWorkPoW[Proof of Work PoW]
DecentralizedAcyclicGraph -->|is a type of data structure for a|Blockchain[Blockchain]
Exchange -->|can host for user|Wallet[Wallet]
Exchange -->|provides|FiatGateway[Fiat Gateway]
Exchange -->|submits|Transaction[Transaction]
HardFork -->|resolved via|Consensus[Consensus]
HardFork -->|results in a new|MainChain[Main Chain]
MainChain -->|receives transactions from|BeaconChain[Beacon Chain]
Miner -->|can be a member of|MiningPool[Mining Pool]
Miner -->|can create a|HardFork[Hard Fork]
Miner -->|can create a|SoftFork[Soft Fork]
Miner -->|creates next|Block[Block]
Miner -->|earns|MiningReward[Mining Reward]
Miner -->|reads from|Mempool[Mempool]
MiningPool -->|can create a|HardFork[Hard Fork]
MiningPool -->|can create a|SoftFork[Soft Fork]
MiningPool -->|creates next|Block[Block]
MiningPool -->|earns|MiningReward[Mining Reward]
MiningPool -->|reads from|Mempool[Mempool]
Node -->|executes|SmartContract[Smart Contract]
Node -->|hosts|BlockchainNetwork[Blockchain Network]
ShardChain -->|sends transactions to|BeaconChain[Beacon Chain]
SmartContract -->|makes use of|Oracle[Oracle]
Transaction -->|contains a|TransactionFee[Transaction Fee]
Transaction -->|is sent to|Mempool[Mempool]
