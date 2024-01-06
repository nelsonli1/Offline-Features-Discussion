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

### Definitions

| Term                                     | Definition                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Authentication                           | Process of verifying and confirming the identity of a user, entity, or system attempting to access or engage in a transaction within the CBDC payment system                                                                                                                                                                                                                                                                                         |
| Authorization                            | Process of granting official permission or approval for a specific action                                                                                                                                                                                                                                                                                                         |
| B2B                                      | Business-to-business                                                                                                                                                                                                                                                                                                                                                               |
| B2C                                      | Business-to-consumer                                                                                                                                                                                                                                                                                                                                                               |
| CBDC                                     | Central bank digital currency                                                                                                                                                                                                                                                                                                                                                     |
| CBDC payment system                      | Comprehensive and integrated infrastructure established by the central bank to facilitate the issuance, distribution, and management of a nation's Central Bank Digital Currency (CBDC)                                                                                                                                                                                                                                                         |
| Clearing                                 | All activities from the time a commitment is made for a transaction until it is settled                                                                                                                                                                                                                                                                                          |
| Counterfeit                              | Made in imitation of something of value or importance with the intention to deceive or defraud                                                                                                                                                                                                                                                                                  |
| Cryptocurrency                           | A digital currency in which transactions are verified and records maintained by a decentralized system using cryptography, rather than by a centralized authority                                                                                                                                                                                                                  |
| Cryptographic key                        | A piece of information, usually a sequence of numbers, letters or symbols, used in encryption and decryption processes within cryptographic algorithms. It serves as a secret parameter that controls the transformation of plaintext (unencrypted data) into ciphertext (encrypted data) and vice versa. The security of encrypted data relies on the strength and secrecy of the key                                                                    |
| Cardholder verification method (CVM)     | A mechanism by which the cardholder proves that they are the rightful user of the card. Often implemented using a PIN or biometric                                                                                                                                                                                                                                                 |
| Double spending                          | The act of sending a transaction containing inputs that have already been spent in an attempt to commit fraud on the network                                                                                                                                                                                                                                                      |
| Failed                                   | Outcome of a transaction attempt that did not successfully complete according to the intended process                                                                                                                                                                                                                                                                         |
| Fully offline system                     | System in which the payer and payee do not need to connect to a ledger system (though there could be a local on-device ledger) to complete a payment, and any value exchanged is immediately transferred to the payee such that they can spend it at the end of the value transfer (settlement occurs offline). Both payer and payee can stay fully offline without limitation in time.                                                         |
| Hardware-based Security                  | Hardware-based security protects an endpoint from malicious threats by relying on specific hardware components (or devices). Endpoint software relies on these hardware components to oppose any alteration or tampering.                                                                                                                                                                                                                    |
| Information transfer channel              | Medium used to transfer transaction information between the involved parties.                                                                                                                                                                                                                                                                                                       |
| Near Field Communication (NFC)           | Short-range wireless communication technology that enables data exchange between devices when they are in close proximity. High Frequency of 13.56 MHz. Range: 10cm. Protocols: The ISO/IEC 14443 and ISO/IEC 18092 standards.                                                                                                                                                                                                                 |
| RFID                                     | Radio Frequency Identification. Range, frequency, power, protocols may vary. TBD: Work on finding RFID compatible with our product and purpose.                                                                                                                                                                                                                                      |
| QR Codes                                 | Two-dimensional barcodes that can store various payment details.                                                                                                                                                                                                                                                                                                                  |
| BLE                                      | Power-efficient version of Bluetooth for short-range transfer of information (100m)                                                                                                                                                                                                                                                                                              |
| Satellite Communication                  | Transmitting information through satellites.                                                                                                                                                                                                                                                                                                                                     |
| Intermittently offline system            | Similar to fully offline, a system in which the payer and payee do not need to connect to a ledger system to complete a payment, and any value exchanged is immediately transferred to the payee such that they can spend it at the end of the value transfer (settlement occurs offline). However, risk parameters will at some point limit the ability of purses to transact, and a purse will have to synchronize with the central system intermittently to continue functioning.              |
| Irreversible                             | Condition where a process, especially a financial transaction, cannot be reversed or undone after completion. This term tends to focus on the technical aspect, highlighting the secure recording of the transaction within the system, ensuring its integrity and immutability.                                                                                                                                                             |
| Irrevocable                              | State where a transaction, decision, or action cannot be revoked, canceled, or changed once initiated. Carries legal implications, binding parties to the terms of a transaction and emphasizing a commitment that cannot be withdrawn.                                                                                                                                                                                                        |
| Key                                      | ? (general key is too broad of a term)                                                                                                                                                                                                                                                                                                                                           |
| Ledger                                   | A collection of financial accounts of a particular type. For CBDC payments, this is the collection of transactions                                                                                                                                                                                                                                                                |
| Ledger system                            | A system or set of systems hosting ledgers. The term specifically does not imply the use of any particular type of technology.                                                                                                                                                                                                                                                    |
| Merchant                                 | Business or entity that provides goods or services and may accept CBDC as a form of payment.                                                                                                                                                                                                                                                                                       |
| Offline                                  | Not controlled by or directly connected to a computer or external network. For CBDC, this refers to being disconnected from CBDC ledger systems, not necessarily disconnected from communication networks                                                                                                                                                                         |
| Password                                 | A protected/private string of letters, numbers, and/or special characters used to authenticate an identity or to authorize access to data online                                                                                                                                                                                                                                    |
| Payee                                   | Entity or individual acting as a recipient or beneficiary of a CBDC payment                                                                                                                                                                                                                                                                                                        |
| Payer                                   | Entity or individual acting as the party that initiates and authorizes a CBDC payment                                                                                                                                                                                                                                                                                               |
| Payment request                          | Message instruction sent from the payee to the payer consisting of transaction information such as amount, payee details, and other information, requesting the payer to initiate a transfer of value to the payee                                                                                                                                                                  |
| Payment instruction                       | Message instruction sent from the payer to the payee consisting of transaction information like amount, payee details                                                                                                                                                                                                                                                             |
| Payment authorization                    | Process of granting approval for the execution of a payment transaction within the CBDC payment system on behalf of the payer                                                                                                                                                                                                                                                     |
| Payment Service Provider                  | Offers support to merchants for accepting payments.                                                                                                                                                                                                                                                                                                                               |
| Pending                                  | Transaction status indicating a period between the payment authorization and the settlement                                                                                                                                                                                                                                                                                      |
| Personal Identification Number (PIN)      | A protected/private numeric code used by the payer during the payment authentication process                                                                                                                                                                                                                                                                                      |
| Proxy                                   | Offline transaction record when immediate online transactions are not possible. The proxy needs to be authenticated/validated for the transaction to be settled.                                                                                                                                                                                                               |
| Pull payment                             | A transaction initiated by the payee pre-authorized by the payer.                                                                                                                                                                                                                                                                                                                 |
| Push payment                             | A transaction initiated by the payer                                                                                                                                                                                                                                                                                                                                             |
| Settlement                               | Irrevocable and irreversible finalization of a transaction                                                                                                                                                                                                                                                                                                                        |
| Staged Offline                           | Where the payer and payee do not need to connect to a ledger system to exchange value, but the value exchanged is not finally settled on the payee until the payee connects to the ledger system. Value transferred to the payee cannot be spent until this second stage of online settlement has occurred.                                                                                                                   |
| Supplier                                 | A merchant providing B2B services or selling goods to other merchants                                                                                                                                                                                                                                                                                                             |
| SIM Card                                 | A smart card inside a mobile phone that carries an identification number unique to the owner, stores personal data, and prevents operation if removed. SIM cards may be secure elements.                                                                                                                                                                                          |
| Tamper-proof                             | The capability of any object to resist attempts to modify it. Detection of tampered data is possible by storing their hash function along with them, as even small modifications in the original data result in different values of their hash.                                                                                                                                                                                                       |
| Tamper-resistant device                   | The device that enables Tamper-proof transactions. To do that, the device itself should be resistant to malicious modification of the device.                                                                                                                                                                                                                                       |
| Transaction history                       | Record of the transactions made by the user. Information contained for transactions may contain different information depending on the user type (e.g., merchant, central bank, etc.)                                                                                                                                                                                              |
| Transaction Status                       | State of the payment transaction. Could be settled, pending, or failed.                                                                                                                                                                                                                                                                                                            |
| Transfer of Value                        | Change ownership or control of value, moved from one entity (payer) to another entity (payee) as part of a transaction                                                                                                                                                                                                                                                            |
| Transaction                              | Exchange or interaction involving the transfer of value between two or more parties within the CBDC payment system                                                                                                                                                                                                                                                               |
| User device                              | A device in the possession of the user which enables them to make offline payments. This could be a smartphone, a smart card, a key fob, a feature phone, or some other piece of technology that provides them with the means to make an offline payment.                                                                                                                                 |
| Value transfer mechanism                 | Any system, mechanism, or network of people that receives money for the purpose of making the funds or an equivalent value payable to a third party in another geographic location, whether or not in the same form.                                                                                                                                                                  |
| Value Transfer Protocol                   | A protocol designed to transport value between two endpoints.                                                                                                                                                                                                                                                                                                                    |
| Value                                    | Monetary worth or financial significance associated with a transaction or asset representing the amount of currency or digital currency being transferred from the payer to the payee in a given transaction.                                                                                                                                                                           |
| Wallet                                   | Any mechanism that can be used to store digital assets (tokens). A cold wallet is a hardware device and can be operated offline, while a hot wallet is an online service based on web resources (and can be operated only by online users).                                                                                                                                                                                                           |


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

# User Stories

## Auditors
- As an auditor, I would like to get all the transaction records of a merchant so that I could determine whether or not a company's financial information is presented fairly. I want all the transactions to be traceable and to have details like transaction amount, timestamp and involved parties in an organized view.
- As an auditor I would like to be able to easily compare the a merchant’s internal records to the central bank records to ensure that both reconcile.
- As an auditor, I want access to a centralized system that facilitates efficient resolution of transaction disputes, ensuring accurate reporting and audit trail documentation.

### Interface Requirements
- Dashboard for overviewing all offline transactions - with filters for dates, users, etc.
- Status indicators of synchronization with the central server and settlements.
- Timestamps, parties involved and user identifiers for every action.
- Role-based access controls.

## Central Bank System Administrator
- As a central bank administrator, I would like to have real-time visibility of all transactions for monitoring purposes to detect anomalies, ensure minimal downtime for users, preventing potential system issues (e.g. double spending) of the CBDC offline payment system.
- As a central bank administrator, I would like to have a real-time visibility of funds in the accounts to monitor and detecting anomalies.
- As a central bank administrator, I need to receive alerts for transactions that exceed predefined thresholds or exhibit suspicious patterns.
- As a central bank administrator, I would like users to synchronize their accounts on a regular basis to improve traceability of funds and security.
- As a central bank administrator, I would like to have the information about the owner of a CBDC account for financial security, fraud prevention and targeted financial assistance.

### Interface Requirements
- Dashboard for Real-Time Monitoring: Provide an interactive dashboard that displays real-time data on CBDC transactions and currency flow which enables quick decision-making and immediate response to any abnormalities or critical issues in the system.
- Integration Capabilities: Ensure the interface can integrate seamlessly with other financial systems, databases, and external APIs to promote interoperability and efficient data exchange, enhancing the system's utility and functionality.
- Backup and Recovery Systems: Implement robust backup and disaster recovery solutions that ensure data integrity and system availability in case of system failures or other disruptions.

## Central Bank as the Regulator
- As a central bank regulator, I would like to have a real-time visibility of all transactions for regulatory purposes so that I can maintain control, detect anomalies and ensure policy compliance, ensuring stability of the financial system.

### Interface Requirements
- Reporting and Compliance Tools: Include automated reporting tools for compliance with regulatory requirements and easy generation of financial reports. Streamlines compliance processes and ensures adherence to regulatory standards. (e.g. Manual inspection when the system detects a transfer that involves large amount of fund).

## Government Authority Responsible for Distributing Emergency Funds
- As a government official, I would like to be able to transfer funds in a timely manner in the event of an emergency to individuals or businesses so that they can use the funds to purchase basic necessities.

### Interface Requirements
- The ability to transfer CDBC to a large group of users in a short period of time, without requiring existing infrastructure.
- The possibility of transferring CDBC across and within different segments of the government.

## Online Merchants
- As a merchant, I want to be able to accept offline CBDC payments from users remotely.
- As a subscription services provider, I want to be able to request recurring payments to manage subscription services to customers.
- As a merchant, I want to have a safety period to approve purchases until the transaction is settled or some mechanism to recover value in case of a failed transaction.
- As a merchant, I would like to be notified of transaction status prior to approving the purchase.
- As a merchant, I want to quickly be able to refund a customer (make a payment to the customer) when they return their purchase.

### Interface Requirements
- Overviewing all offline transactions - Total revenue, items sold, timestamp for each transaction, identifier information for each transaction.
- A subscription payment system. When a user agrees to use your service and pays the fee periodically, the system should be able to automatically transfer this money.
- It should be easy to trace and manage each customer purchase record to provide customer service, such as refund, exchange and upgrade.
- Notification system to ensure customers that the payment is settled.
- Mechanism to initiate refund on purchases that have been returned/damaged during delivery process.
- Database for keeping track record of all offline transactions.

## Payee
- As a payee, I want a simple user-friendly interface for receiving offline CBDC transactions. The process should require the least effort as possible on my behalf.
- As a payee, I want a status notification for the offline CBDC transaction that indicates whether the payment succeeded, is still pending, or failed.
- As a child, I want to receive money from my parents to buy lunch at school without having to request it.
- As a payee, I would like to receive emergency CBDC funds in the case of natural disaster events so that I can purchase items of immediate need.
- As an individual, I want to request money from my other friends to pay me back for lunch.
- As a payee, I want to be able to transfer money from my online wallet to my offline wallet from both CBDC and conventional form of money.
- As a payee, I want to be able to deposit excess funds onto a separate device stored in a secure location.

### Interface Requirements
- Transaction overview: transaction amount, timestamp, status (value received/settled).
- Payer Information (identifier/name), transaction ID, purpose of transaction (description).
- Confirmation prompts for important actions.
- Export functionality to store transaction record locally on the device.
- Help section in case something goes wrong.

## Payer
- As a payer, I want a user-friendly interface for initiating and authorizing offline CBDC transactions securely.
- As a payer, I would like to be able to recover the value of my CBDC funds in case if I lose my wallet.
- As a parent, I want to give money to my child to buy lunch at school without having the child initiate the transaction.
- As an individual with a phone plan, I would like to pay my phone bill each month using offline CBDC without having to authorize the transaction each time.
- As an online shopper, I want to purchase items online using my offline CBDC wallet remotely.
- As an in-person shopper, I want to purchase items in-store using CBDC through a tap-to-pay method.
- As an online or in-person shopper, I would like to be able to initiate a chargeback process in situations where requesting a refund is not a viable option.
- As a payer, I want explicit confirmation prompts for the verification of the party on the receiving end so that my money doesn’t disappear.
- As a payer, I want to be able to quickly and independently add funds to my account from a funds storage at home so that I have enough funds to make a payment.
- As a payer, I want to be able to freely switch between various payment methods online and in person at the point of transaction.
- As a payer, I want to be able to go to an ATM to top up my offline wallet or withdraw physical cash from my offline wallet.

### Interface Requirements
- Confirmation for the authentication of the payee (probably need a certificate mechanism for that) (subject to discussion).

## Physical Merchants
- As a merchant, I want to accept offline payments from customers at the store through a tap-to-pay method.
- As a merchant, I want to integrate CBDC payment acceptance with my existing payment accepting devices.
- As a merchant, I want a CBDC payment system to have the same user identification across multiple approved devices so that all my income goes to the same account.
- As a merchant, I want a mechanism to authorize my employees to accept the transactions on my devices.
- As a merchant, I want a legal mechanism to settle pending/failed transactions or disputes.
- As a customer service representative, I want the ability to retrieve and review detailed transaction histories for customer inquiries, ensuring efficient customer support by providing representatives with the necessary information to address customer inquiries.
- As a manager, I would like the CBDC payment system to be integrated with other systems including ERP, Accounting ensuring single source of truth and consistency across multiple systems.
- As an owner, I would like to authorize managers to handle transactions on my behalf (payments, reimbursements, etc.).
- As an owner, I would like real-time updates on unsuccessful transactions to notify customers and assist customers.

### Interface Requirements
- All transactions overview: cumulative statistics about transactions.
- Transaction overview: transaction amount, timestamp, status (value received/settled).
- Payer Information (identifier/name), transaction ID, purpose of transaction (description).
- Needed in case of insufficient funds (i.e., buying stuff with a cheque in Stan’s example).
- Refund mechanism to reimburse payees for returned/damaged goods.

## Police Authority
- As a police officer responsible for investigating criminal cases, I would need to get the transaction records of the suspect including the sender and the receiver so that I could use them as evidence. (Should be able to find the person connected to a CBDC account).

### Interface Requirements
- Authorization to overview transaction history of the individual being investigated.
- Ability to follow the money spent/received by the individual

## Tax Authority
- As a government authority, I want to be able to see the transaction record of a person's financial history, and ensure that they adhere to legal and compliance requirements, preventing tax evasion.
