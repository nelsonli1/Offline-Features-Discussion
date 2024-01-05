# Offline Features Discussion

### Feature objectives

- Inclusion
- Resilience
- Convenience 
- Security
- Privacy



### Personas
- Auditors - People or organization that conduct audits
- Central bank as the operator of the system - As an operator, the central bank’s responsibility is ensuring smooth and efficient operation of the payment system.
- Central bank as the regulator - As a regulator, the central bank's primary responsibility is to oversee and maintain the stability, efficiency, and integrity of the financial system, which includes formulating monetary policy, supervising banks, ensuring consumer protection, and managing systemic risks.
- Online merchants - The merchants that hold their business online and should be able receive the payment regardless of the physical distance with the customer.
- Payee - a recipient or beneficiary of a CBDC payment
- Payer - entity or individual who initiates and authorizes a CBDC payment
- Physical merchants - The merchants that hold their business offline and should be able to receive the payment in the same physical location with the customers.
- Police authority - A police authority refers to a government body or organization responsible for enforcing laws related to financial crimes, such as fraud and money laundering associated with CDBC transactions.
- Tax authority - An organization with official responsibility for collecting tax.

### Definition
- **Authentication:** Process of verifying and confirming the identity of a user, entity, or system attempting to access or engage in a transaction within the CBDC payment system.

- **Authorization:** Process of granting official permission or approval for a specific action.

- **B2B:** Business-to-business.

- **B2C:** Business-to-consumer.

- **BLE:** Bluetooth low energy.

- **CBDC:** Central bank digital currency.

- **Clearing:** All activities from the time a commitment is made for a transaction until it is settled.

- **Counterfeit:** Made in imitation of something of value or important with the intention to deceive or defraud.

- **Cryptocurrency:** A digital currency in which transactions are verified and records maintained by a decentralized system using cryptography, rather than by a centralized authority.

- **Cryptographic Key:** A piece of information, usually a sequence of numbers, letters, or symbols, used in encryption and decryption processes within cryptographic algorithms. It serves as a secret parameter that controls the transformation of plaintext (unencrypted data) into ciphertext (encrypted data) and vice versa. The security of encrypted data relies on the strength and secrecy of the key.

- **Cardholder Verification Method (CVM):** A mechanism by which the cardholder proves that they are the rightful user of the card. Often implemented using a PIN or biometric.

- **Double Spending:** The act of sending a transaction containing inputs that have already been spent in an attempt to commit fraud on the network.

- **Fully Offline System:** System in which the payer and payee do not need to connect to a ledger system (though there could be a local on-device ledger) to complete a payment, and any value exchanged is immediately transferred to the payee such that they can spend it at the end of the value transfer (settlement occurs offline). Both payer and payee can stay fully offline without limitation in time.

- **Hardware-based Security:** Hardware-based security protects an endpoint from malicious threats by relying on specific hardware components (or devices). Endpoint software relies on these hardware components to oppose any alteration or tampering.

- **Information Transfer Channel:** Medium used to transfer transaction information between the involved parties.

- **Near Field Communication (NFC):** Short-range wireless communication technology that enables data exchange between devices when they are in close proximity. High Frequency of 13.56 MHz. Range: 10cm. Protocols: The ISO/IEC 14443 and ISO/IEC 18092 standards.

- **RFID:** Radio Frequency Identification. Range, frequency, power, protocols may vary. TBD: Work on finding RFID compatible with our product and purpose.

- **QR Codes:** Two-dimensional barcodes that can store various payment details.

- **Irreversible:** Condition where a process, especially a financial transaction, cannot be reversed or undone after completion. This term tends to focus on the technical aspect, highlighting the secure recording of the transaction within the system, ensuring its integrity and immutability.

- **Irrevocable:** State where a transaction, decision, or action cannot be revoked, canceled, or changed once initiated. Carries legal implications, binding parties to the terms of a transaction and emphasizing a commitment that cannot be withdrawn.

- *Key:* ?

- **Ledger:** A collection of financial accounts of a particular type. For CBDC payments, this is the collection of transactions.

- **Ledger System:** A system or set of systems hosting ledgers. The term specifically does not imply the use of any particular type of technology.

- **Merchant:** Business or entity that provides goods or services and accepts CBDC payments.

- **Offline:** Not controlled by or directly connected to a computer or external network. For CBDC, this refers to being disconnected from CBDC ledger systems, not necessarily disconnected from communication networks.

- *Password:* A protected/private string of letters, numbers, and/or special characters used to authenticate an identity or to authorize access to data online.

- **Payee:** A recipient or beneficiary of a CBDC payment.

- **Payer:** Entity or individual who initiates and authorizes a CBDC payment.

- **Payment Request:** Message instruction sent from the payee to the payer consisting of transaction information such as amount, payee details, and other information, requesting payer to initiate a transfer of value to the payee.

- **Payment Instruction:** Message instruction sent from the payer to the payee consisting of transaction information like amount, payee details.

- *Payment Authorization:* Process of granting approval for the execution of a payment transaction within the CBDC payment system on behalf of the payer.

- **Payment Service Provider:** Offers support to the merchants for accepting payments.

- **Personal Identification Number (PIN):** A protected/private numeric code used by the payer during the payment authentication process.

- *Proxy:* Offline transaction record when immediate online transactions are not possible. The proxy needs to be authenticated/validated for the transaction to be settled.

- **Pull Payment:** A transaction initiated by the payee pre-authorized by the payer.

- **Push Payment:** A transaction initiated by the payer.

- **Settlement:** Irrevocable and irreversible finalization of a transaction.

- **Staged Offline:** Where the payer and payee do not need to connect to a ledger system in order to exchange value, but the value exchanged is not finally settled on the payee until the payee connects to the ledger system. Value transferred to the payee cannot be spent until this second stage of online settlement has occurred.

- **Supplier:** A merchant providing B2B services or selling goods to other merchants.

- **SIM Card:** A smartcard inside a mobile phone that carries an identification number unique to the owner, stores personal data, and prevents operation if removed. SIM cards may be secure elements.

- **Tamper-proof:** The capability of any object to resist attempts to modify it. Detection of tampered data is possible by storing their hash function along them, as even small modifications in the original data result in different values of their hash.

- **Tamper-resistant device:** The device that enables Tamper-proof transactions, to do that the device itself should be resistant to malicious modification of the device.

- **Transaction history:** Record of the transactions made by the user. Information contained for transactions may contain different information depending on the user type (e.g. merchant, central bank, etc.)

- **Transfer of Value:** Change ownership or control of value, moved from one entity (payer) to another entity (payee) as part of a transaction

- **Transaction:** exchange or interaction involving the transfer of value between two or more parties within the CBDC payment system

- **User device:** A device in the possession of the user which enables them to make offline payments. This could be a smartphone, a smartcard, a key fob, a feature phone or some other piece of technology that provides them with the means to make an offline payment.

- **Value transfer mechanism:** Any system, mechanism or network of people that receives money for the purpose of making the funds or an equivalent value payable to a third party in another geographic location, whether or not in the same form.

- **Value Transfer Protocol:** A protocol designed to transport value between two endpoints.

- **Value:** monetary worth or financial significance associated with a transaction or asset representing the amount of currency or digital currency being transferred from the payer to the payee in a given transaction.

- **Wallet:** Any mechanism that can be used to store digital assets (tokens). A cold wallet is a hardware device and can be operated offline, while a hot wallet is an online service based on web resources (and can be operated only by online users). 



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



