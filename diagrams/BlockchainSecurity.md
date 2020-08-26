```mermaid
graph LR
BlockchainSecurity(BlockchainSecurity)
34Attack -->|type of|AttackAgainstConsensusMechanisms[Attack Against Consensus Mechanisms]
51Attack -->|type of|AttackAgainstConsensusMechanisms[Attack Against Consensus Mechanisms]
AttackAgainstExchanges -->|gains access to|HostedWallet[Hosted Wallet]
ChainLocks -->|defense against|51Attack[51% Attack]
ChainLocks -->|defense against|AttackAgainstConsensusMechanisms[Attack Against Consensus Mechanisms]
CredentialStuffingAttack -->|results in|PasswordTheftAttack[Password Theft Attack]
DelayedProofofWorkdPoW -->|defense against|51Attack[51% Attack]
DelayedProofofWorkdPoW -->|defense against|AttackAgainstConsensusMechanisms[Attack Against Consensus Mechanisms]
MergedMining -->|defense against|51Attack[51% Attack]
MergedMining -->|defense against|AttackAgainstConsensusMechanisms[Attack Against Consensus Mechanisms]
PasswordTheftAttack -->|gains access to|ExchangeAccount[Exchange Account]
PasswordTheftAttack -->|gains access to|HostedWallet[Hosted Wallet]
PasswordTheftAttack -->|gains access to|Wallet[Wallet]
PenaltySystem -->|defense against|51Attack[51% Attack]
PenaltySystem -->|defense against|AttackAgainstConsensusMechanisms[Attack Against Consensus Mechanisms]
PirlGuard -->|defense against|51Attack[51% Attack]
PirlGuard -->|defense against|AttackAgainstConsensusMechanisms[Attack Against Consensus Mechanisms]
Two-FactorAuthentication -->|defense against|PasswordTheft[Password Theft]
Two-FactorAuthenticationviaBiometrics -->|defense against|PasswordTheft[Password Theft]
Two-FactorAuthenticationviaBiometrics -->|defense against|SimSWAP[Sim SWAP]
Two-FactorAuthenticationviaEmail -->|defense against|PasswordTheft[Password Theft]
Two-FactorAuthenticationviaEmail -->|defense against|SimSWAP[Sim SWAP]
Two-FactorAuthenticationviaHardwareToken -->|defense against|PasswordTheft[Password Theft]
Two-FactorAuthenticationviaHardwareToken -->|defense against|SimSWAP[Sim SWAP]
Two-FactorAuthenticationviaOneTimeCode -->|defense against|PasswordTheft[Password Theft]
Two-FactorAuthenticationviaPhoneCall -->|defense against|PasswordTheft[Password Theft]
Two-FactorAuthenticationviaPhysicalMail -->|defense against|PasswordTheft[Password Theft]
Two-FactorAuthenticationviaSMS -->|defense against|PasswordTheft[Password Theft]
Two-FactorAuthenticationviaSoftwareToken -->|defense against|PasswordTheft[Password Theft]
Two-FactorAuthenticationviaSoftwareToken -->|defense against|SimSWAP[Sim SWAP]