# Offline Features Discussion

### Feature objectives

- Inclusion
- Resilience
- Convenience 
- Security
- Privacy

### Persona

- **Auditors**: People or organization that executes audits on merchant’s financial information

- **Central bank as the operator of the system**: As an operator, the central bank’s responsibility is ensuring smooth and efficient operation of the CBDC payment system, which includes managing clearing and settlement processes for transactions

- **Central bank as the regulator**: As a regulator, the central bank's primary responsibility is to oversee and maintain the stability, efficiency, and integrity of the financial system, which includes formulating monetary policy, supervising banks, ensuring consumer protection, and managing systemic risk

- **Online merchants**: Merchants that hold their business online and should be able to receive the payment regardless of the physical distance with the customer

- **Payee**: Entity or individual acting as a recipient or beneficiary of a CBDC payment

- **Payer**: Entity or individual acting as the party that initiates and authorizes a CBDC payment

- **Physical merchants**: Merchants that hold their business offline and should be able to receive the payment in the same physical location with the customers

- **Police authority**: A government body or organization responsible for enforcing laws related to financial crimes, such as fraud and money laundering associated with CDBC transactions

- **Tax authority**: Government agency or organization responsible for overseeing and implementing taxation policies within a specific jurisdiction. The primary functions of a tax authority include assessing, collecting, and enforcing taxes on individuals, businesses, and other entities


### Design Considerations:
| Name                               | Description                                                                                                                         | Benefits                                                                                                                    | Drawbacks                                                                                                                              |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------|
| **Transaction History Management** | Offline devices can either record full transaction history offline or record partial transaction history with ability to synchronise history online | Settlements can occur when money or wallet is lost through tracing the individual's transaction history, improving security | The transaction history is stored offline or online and users have the risk of losing their privacy.                                     |
| **Synchronisation Details**        | When connected online, devices can either update the balance along with the full transaction history or update just the balance of the card  | - Full transaction history provides more traceability, improving security<br>- Balance enables anonymity<br>- Prevents forgeability | Privacy is compromised as more details are stored onto the database.<br>Requires connection to an online server at some point.          |
| **Mode of Offline Payment**        | Offline payments can be fully offline, intermittently offline, or staged offline                                                   | Moving towards a fully offline system can increase inclusion, convenience, privacy<br>Staged offline system can improve security<br>Can be used in case of natural disasters/other emergency situations. | Trade-off related to privacy and security.<br>Potential issues with managing settlements in a fully offline system, compromising security |
| **Hardware**                       | Offline payment system can run on standalone hardware device, hardware depending on existing hardware, or fully software on existing hardware | - Secured hardware adds protection<br>- Attachments on existing hardware increase convenience<br>- Software-based solutions are convenient | - Production costs for standalone hardware<br>- Weakened security with software systems<br>- Assumes user ownership of mobile devices   |
| **Offline Registry**               | An offline database to cross-reference user base                                                                                    | Written record and assurance of sending money to the correct person, increased security.                                      | - Needs regular updates<br>- No track of new accounts in emergencies<br>- Privacy concerns with public information                    |
| **Frequency of Cryptographic Key Generation** | Keys generated once or at regular intervals                                                                                         | Improves security, limiting potential misuse and fraud.                                                                      | - Inconvenient for frequent key changes<br>- Hindrance for non-tech-savvy individuals                                                  |
| **One-Time-Use Security Token for Transaction** | Use of digital and blind signatures, tokens with the same serial number to buyer and seller                                         | - Prevents double spending<br>- Ensures only the intended payee can receive the value                                        | TBD                                                                                                                                    |
| **Remote Ledger to Record Ownership** | Centralised record of ownership of each token                                                                                       | - Detects unauthorised tokens<br>- Prevents double-spending                                                                  | Privacy and anonymity concerns                                                                                                         |
| **Exchange of Value Process**      | Process involving PIN number, payee unique number, transaction amount, and a random generated number                                | Guarantees correct payee and amount                                                                                          | Cumbersome process of entering a series of numbers                                                                                     |
| **Discontinuation of Obsolete/Damaged Devices** | Replacement of obsolete/damaged offline payment devices                                                                             | Improves resilience with a process for recovering value                                                                      | Security may be compromised, increasing risk of double spending                                                                        |
| **Push Mechanism**                 | Transactions initiated to send money without the recipient's request                                                               | Emulates convenience of online payments and cash<br>Useful in emergencies or for parental allowances                         | Buyer might send less than the agreed amount in sales transactions                                                                     |
| **Pull Mechanism**                 | Transactions initiated by requesting a value to be paid by another user                                                            | Allows payees to request the agreed amount of money                                                                          | Requires a payment request to be initiated                                                                                             |
| **Value Transfer Mechanism**       | Options include NFC, BLE, Text-based, Audio signal-based, Satellite technology, QR Code                                            | - Various methods cater to different needs and situations<br>- NFC and BLE are secure for certain contexts<br>- Satellite and QR codes offer unique advantages | - Distance and security limitations of NFC and BLE<br>- Cost of satellite transmission<br>- QR codes vulnerable to tampering            |
| **PIN Verification for Transactions** | Unique user-specific PIN for transactions                                                                                          | Ensures only the wallet owner can transact                                                                                   | Cumbersome for users to enter PINs frequently                                                                                          |
| **Torn Transaction**               | Issue where value is removed from payer but not updated on payee                                                                   | Prevents malicious users from double-spending                                                                                | Difficult to recover lost value in offline systems                                                                                     |


#### Policy Considerations

- What should be the block list management process to prevent payments from lost / stolen devices?
- What should be the transaction limits for offline transactions?
- How do we define the settlement process?
- How many devices can be issued at the same time?
- What is the process for issuing new digital wallets? What kind of documentation is required from both merchants and consumers?
- To what extent should the transactions be tracked?
- How many devices can an individual have at once?
- How long before we blacklist a card? Should we return the money after blacklisting a card?
- Insurance policy for returning money in case of a natural disaster, fire, etc?
- What policy should be required to prevent double spending?



