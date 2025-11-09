# Literature Survey: Blockchain for Secure Transmission and Storage of Sensitive Documents

## Executive Summary

This literature survey examines 20+ research and conference papers focusing on blockchain technology applications for secure transmission and storage of sensitive documents. The survey covers healthcare records management, legal document security, government applications, cloud storage security, and various cryptographic protocols that enhance document security through blockchain implementation.

**Note on Author Information:** This survey includes author names where they were readily available from academic databases (PubMed, ACM Digital Library, Springer, etc.). Some papers, particularly industry whitepapers and technical reports, are marked as "(Authors to be confirmed)" as complete author information was not accessible in the initial search. For academic research purposes, readers are encouraged to access the original publications through their respective databases for complete authorship details.

---

## 1. Healthcare and Medical Records Management

### 1.1 Survey on Blockchain-Based Data Storage Security for Android Mobile Applications
**Authors:** Hussam Saeed Musa, Moez Krichen, Adem Alpaslan Altun, Meryem Ammi  
**Source:** Sensors (MDPI) / PMC - NCBI  
**Year:** 2023

This research investigates the integration of blockchain technology to enhance the security of Android mobile app data storage, noting that blockchain holds significant potential to improve data security and reliability despite challenges such as scalability, performance, cost, and complexity. The study emphasizes that mobile apps storing sensitive information such as personal identification documents, financial information, and medical records have made data storage security a critical concern.

**Key Contributions:**
- Comprehensive review of blockchain integration in mobile app security
- Analysis of encryption techniques versus blockchain effectiveness
- Focus on privacy protection through encryption and digital signatures

---

### 1.2 Blockchain-Based Medical Records Secure Storage and Medical Service Framework
**Authors:** Y. Chen, S. Ding, Z. Xu, H. Zheng, S. Yang  
**Source:** Journal of Medical Systems  
**Year:** 2018

This paper designs a storage scheme to manage personal medical data based on blockchain and cloud storage, presenting a service framework for sharing medical records while analyzing the characteristics of the medical blockchain through comparison with traditional systems. The research emphasizes that accurate and complete medical data are valuable assets for patients, and privacy protection along with secure storage of medical data are crucial issues during medical services.

**Key Features:**
- Combined blockchain and cloud storage architecture
- Attribute-based encryption for access control
- Immutable and verifiable transaction records

---

### 1.3 MedBlock: Efficient and Secure Medical Data Sharing Via Blockchain
**Authors:** Kai Fan, Shangyang Wang, Yanhui Ren, Hui Li, Yintang Yang  
**Source:** Journal of Medical Systems  
**Year:** 2018

This system proposes MedBlock to handle patients' information, where the distributed ledger allows efficient EMRs access and retrieval, and the improved consensus mechanism achieves consensus of EMRs without large energy consumption and network congestion. The research addresses the difficulty of constructing a summarized EMR for one patient from multiple hospital databases due to security and privacy concerns.

**Key Innovations:**
- Energy-efficient consensus mechanism
- Distributed ledger for EMR access
- Privacy-preserving data sharing protocol

---

### 1.4 Secure and Trustable Electronic Medical Records Sharing using Blockchain
**Authors:** Alevtina Dubovitskaya, Zhigang Xu, Samuel Ryu, Michael Schumacher, Fusheng Wang  
**Source:** AMIA Annual Symposium Proceedings  
**Year:** 2018

The paper presents perspectives on blockchain-based healthcare data management, particularly for EMR data sharing between healthcare providers and for research studies, proposing a framework for managing and sharing EMR data for cancer patient care. Electronic medical records are critical, highly sensitive private information in healthcare that need to be frequently shared among peers, and blockchain provides a shared, immutable and transparent history of all transactions to build applications with trust, accountability and transparency.

**Implementation Details:**
- Prototype developed with Stony Brook University Hospital
- Fine-grained access control over EMR data
- Ensures privacy, security, and availability

---

### 1.5 A Blockchain-Based Secret-Data Sharing Framework for Personal Health Records in Emergency Condition
**Source:** PMC - NCBI  

This paper suggests a healthcare management framework that employs blockchain technology to provide tamper protection, introducing a blockchain-based model for providing dynamic, interoperable, and secure access to medical records while protecting patients' sensitive information. The system employs the Ethereum blockchain by defining smart contracts for affording access control and obfuscation of data and applied cryptographic methods for extra security.

**Special Features:**
- Emergency access protocols without patient approval
- Smart contracts for access permission limitation
- Tracking system for PHR access history

---

### 1.6 Electronic Medical Record Security Sharing Model Based on Blockchain
**Authors:** (Authors to be confirmed - ACM Conference Paper)  
**Source:** ACM Proceedings - International Conference on Cryptography, Security and Privacy  
**Year:** 2019

The paper designs a safe and efficient electronic medical record sharing model based on blockchain, introducing data masking technology and Inter Planetary File System (IPFS) to guarantee the security of medical data while saving resources in blockchain. The model addresses the characteristics of decentralization, security, trustworthiness, collective maintenance, and tamper-proof features suitable for data protection and sharing.

**Technical Approach:**
- Integration with IPFS for distributed storage
- Data masking for sensitive information protection
- Delegated Proof of Stake (DPoS) consensus

---

### 1.7 An Ethereum Blockchain Based Electronic Health Record System for Inter-Hospital Secure Data Sharing
**Authors:** (Authors to be confirmed - ACM Conference Paper)  
**Source:** ACM Proceedings - International Conference on Sustainable Information Engineering  
**Year:** 2020

The implementation of blockchain into medical records enables data to be shared securely between hospitals using Ethereum, where the data stored on the Ethereum blockchain will always be there and can be seen as long as the blockchain network is still online.

**Platform Characteristics:**
- Ethereum-based decentralized applications
- Computer nodes as blockchain participants
- Elimination of third-party intermediaries

---

### 1.8 A Blockchain based Electronic Medical Health Records Framework using Smart Contracts
**Authors:** (Authors to be confirmed - IEEE Conference Paper)  
**Source:** IEEE Conference Publication  
**Year:** 2021

This paper explores the likelihood of representing medical records to ensure data privacy, data accessibility, and data interoperability for healthcare-specific scenarios, addressing protection to ensure data is available.

---

### 1.9 Rechain: A Secured Blockchain-Based Digital Medical Health Record Management System
**Authors:** (Authors to be confirmed - IEEE Conference Paper)  
**Source:** IEEE Conference Publication  
**Year:** 2023

Re-chain is a secure blockchain-based digital medical health record management system developed to solve problems with centralized and traditional systems, based on the Ethereum network and using web3.storage which is an Interplanetary File System for decentralized file storage. The typical method of keeping track of medical records uses paper and centralized systems, which introduces uncertainty and can lead to inaccurate information, identity theft, and lack of accessibility.

---

### 1.10 Que Bian: An Electronic Medical Record Management System on Blockchain
**Authors:** (Authors to be confirmed - ACM Conference Paper)  
**Source:** ACM Proceedings - International Conference on Blockchain Technology and Applications  
**Year:** 2020

This system takes advantage of blockchains' tamper-proof and decentralization properties to develop a robust and secure electronic medical record management system, choosing HyperLedger Fabric as the underlying technical architecture which yields higher throughput and lower latency compared with other blockchains.

---

## 2. Cloud Storage and File Sharing Systems

### 2.1 An Efficient Blockchain-Based Framework for File Sharing
**Authors:** (Authors to be confirmed - Scientific Reports)  
**Source:** Scientific Reports (Nature)  
**Year:** 2024

This paper designs a blockchain-based system architecture for secure sharing of electronic documents, addressing the difficulty of tamper detection and lack of supervision in the entire process of file transfer in the current Internet environment. File sharing has traditionally relied on centralized service architecture resulting in significant maintenance costs, and due to the lack of effective file management systems, instances of sensitive information going out of control and loss of confidentiality have occurred frequently.

**System Architecture:**
- Efficient blockchain model
- Distributed storage system integration
- Asymmetric encryption technology
- Novel consensus mechanism combining DPoS and PBFT

---

### 2.2 An Implementation of Secure Storage Using Blockchain
**Authors:** (Authors to be confirmed - Scientific Temper Journal)  
**Source:** Scientific Temper Journal  

This paper proposes a blockchain-based file storage (BBFS) system that takes advantage of features like immutability, transparency, and security, allowing users to upload unlimited files with data placed in blocks along with username, file size, and file information. The system addresses problems in decentralized file storage where integrity of user data may be compromised, proposing a solution that can be connected with cloud storage to give users a safe place to store and access files that cannot be altered.

---

### 2.3 A Secure, Privacy-Preserving, and Cost-Efficient Decentralized Cloud Storage Framework
**Authors:** (Authors to be confirmed - ScienceDirect)  
**Source:** ScienceDirect  
**Year:** 2024

This paper suggests a blockchain-assisted secure storage and access mechanism to secure sensitive data, where blockchain is used as a trust management entity that verifies user identity, issues Access Control Lists and identity tokens, and records all interactions between users and service providers. The research addresses controlled access failures in preserving privacy of sensitive information stored in the cloud due to insider attacks, breaches of data security, or unauthorized access.

---

### 2.4 Secure Cloud File Sharing Scheme Using Blockchain and Attribute-Based Encryption
**Authors:** (Authors to be confirmed - ScienceDirect)  
**Source:** ScienceDirect  
**Year:** 2023

This paper presents a novel collaboration scheme for secure cloud file sharing using blockchain and attribute-based encryption, where blockchain enables implementation of access control as a smart contract between data owner and users. The encryption key is embedded into a set of coefficients of a polynomial called access polynomial, and the scheme supports fast revocation by means of updating the access polynomial coefficients.

**Security Features:**
- Fast access revocation mechanism
- Smart contract-based access control
- User anonymity preservation
- Subscription key distribution

---

### 2.5 A Secure Blockchain Framework for Healthcare Records Management Systems
**Authors:** (Authors to be confirmed - Healthcare Technology Letters)  
**Source:** Healthcare Technology Letters - Wiley  
**Year:** 2024

The paper proposes a secure blockchain framework for healthcare records management discussing privacy and security concerns related to electronic health records, where data encryption guarantees patient data stays private, preventing illegal individuals from logging on or employing sensitive data. Blockchain technology employs advanced encryption techniques such as asymmetric encryption and hashing which ensures that only authorized parties can access or modify healthcare records, offering superior protection compared to traditional centralized systems.

---

## 3. Legal and Government Document Security

### 3.1 Blockchain for Document Verification and Notarization
**Authors:** (Technical/Industry Paper)  
**Source:** PowerPatent  
**Year:** 2023

Smart contracts are self-executing agreements with predefined rules and conditions that can automate the document verification and notarization process on the blockchain, ensuring that documents are verified consistently and securely. When notarizing documents on the blockchain, it's essential to hash the documents before storing them, creating a unique digital fingerprint of the document that can be used for verification.

**Applications:**
- Land title records management
- Property deed verification
- Legal contract automation
- Reduced risk of fraudulent land claims

---

### 3.2 Revolutionizing Document Security with Blockchain in Government
**Authors:** (Technical/Industry Paper)  
**Source:** Zircon Tech  
**Year:** 2024

By digitizing documents such as land titles and property deeds and recording them on a blockchain, governments can create a transparent and secure system where every change to a title or deed is tracked and permanently recorded. By storing IDs on a blockchain, governments can combat identity theft and unauthorized access to citizen information, with each citizen's identity verified against the blockchain record during transactions requiring identity checks.

**Government Use Cases:**
- National security information protection
- Citizen records management
- Personal identification documents
- Voting system integrity

---

### 3.3 Applying Blockchain in Legal Documents and Certification for Secure Documents
**Authors:** (Technical/Industry Paper)  
**Source:** Deltec Bank and Trust  
**Year:** 2024

Blockchain technology eliminates the need for drawing up contracts when in a courtroom through data verification to avoid fraud, and given the blockchain's data is totally immutable, there do not need to be concerns about tampering with documents. Imagine a world where all case documents were stored in a ledger that could not be tampered with, was highly secure, and could be accessed by all necessary parties - that is precisely what blockchain technology has the potential to do.

**Legal Industry Benefits:**
- Notary services through blockchain startups
- Intellectual property rights management
- Copyright case resolution
- Smart contract execution

---

### 3.4 Blockchain in Legal: A Game Changer for Document Security
**Authors:** (Technical/Industry Paper)  
**Source:** Zircon Tech  
**Year:** 2024

Blockchain is a distributed ledger technology that offers an immutable, secure, and transparent way to record transactions and data - a feature that's incredibly appealing in legal contexts where the integrity and authenticity of documents are paramount. By recording property deeds on a blockchain, every change in ownership becomes part of an indelible ledger, making it easy to verify histories and ownership securely and transparently.

---

### 3.5 Implementing Blockchain for Legal Document Security
**Authors:** (Technical/Industry Paper)  
**Source:** Zircon Tech  
**Year:** 2024

When a document needs to be verified, its hash is recomputed and compared with the hash stored on the blockchain - if the hashes match, the document is confirmed to be unaltered and authentic. Blockchain's decentralized nature makes it resistant to tampering and fraud, where each transaction is encrypted and linked to the previous transaction, creating a secure and unalterable chain.

---

### 3.6 Blockchain Document Signing Platform
**Authors:** (Technical/Industry Paper - CorpoSign)  
**Source:** CorpoSign  
**Year:** 2023

Blockchain can record an exact time stamp/date as well as the identity of the person who signed the document, allowing multiple parties to sign a document using a legally and securely binding process. By storing a document's hash on the blockchain, users can check the document's integrity and authenticity at any time by running it through the same hash function and comparing the resulting hash to the one stored on the blockchain.

---

### 3.7 Use Cases: Blockchain for Public Records and Identity Verification
**Authors:** (Technical/Industry Paper - BlockApps)  
**Source:** BlockApps Inc.  
**Year:** 2024

By distributing the storage and verification of records across a network of nodes, blockchain eliminates single points of failure, making the system more resilient to attacks and data breaches. The immutability of blockchain records is particularly crucial for sensitive documents such as land titles, birth and death certificates, and court records, ensuring the permanence and tamper-resistance of these records.

---

## 4. Cryptographic Protocols and Data Privacy Protection

### 4.1 A Survey on the Application of Blockchain in Cryptographic Protocols
**Authors:** (Authors to be confirmed - Springer)  
**Source:** Cybersecurity - Springer  
**Year:** 2024

Blockchain technology as a solution incorporating decentralization, traceability, programmability, and immutability effectively enhances the security, trustworthiness, operational efficiency, and ensures the security and integrity of data storage in traditional cryptographic protocols. In Wireless Body Area Networks, transmitting sensitive data from users to a central server for processing and storage exposes the information to potential security threats posed by malicious attackers.

**Protocol Applications:**
- Certificateless Authenticated Key Agreement (CLAKA)
- Wireless Body Area Networks security
- Key escrow schemes
- Session key establishment

---

### 4.2 A Systematic Review on Blockchain-Based Access Control Systems in Cloud Environment
**Authors:** (Authors to be confirmed - Journal of Cloud Computing)  
**Source:** Journal of Cloud Computing  
**Year:** 2024

This systematic review examines how blockchain technology can improve cloud access control, grouping suggested papers into 12 different categories and analyzing blockchain-based access control paradigms. The work provides critical analysis of research on blockchain technology in access control systems, focusing on scalability, compatibility, and security challenges.

---

### 4.3 A Study on Blockchain-Based Data Proxy Re-Encryption Privacy Protection
**Authors:** (Authors to be confirmed - ACM Conference Paper)  
**Source:** ACM Proceedings - International Conference on Cryptography, Network Security  
**Year:** 2024

The paper focuses on the problem of storage trustworthiness of edge nodes under the end-edge cloud structure, addressing data susceptibility to attacks and loss, as well as complexity of node interaction in edge scenarios resulting in impaired data accuracy.

**Technical Components:**
- Proxy re-encryption schemes
- Blockchain-based controlled sharing
- Attribute-based proxy re-encryption
- Vehicular communication systems security

---

### 4.4 Design of Blockchain Traceability Mechanism for Data Privacy Protection
**Authors:** (Authors to be confirmed - ACM Conference Paper)  
**Source:** ACM Proceedings - International Conference on IoT and Cloud Computing  
**Year:** 2024

This paper proposes a blockchain data provenance mechanism based on zero-knowledge proof, achieving privacy protection of data provenance by combining blockchain technology and zero-knowledge proof. The mechanism includes three stages: data generation and commitment, data transmission and verification, and data access control, using cryptographic techniques to ensure data privacy and security.

**Performance Characteristics:**
- Superior performance under different data scales
- Lower latency in data transmission and verification
- Enhanced query throughput
- Scalable zero-knowledge proof algorithms

---

### 4.5 Blockchain Distributed Identity Management Model for Cross-Border Data Privacy Protection
**Authors:** (Authors to be confirmed - Journal of Surveillance, Security and Safety)  
**Source:** Journal of Surveillance, Security and Safety  
**Year:** 2023

A distributed identity management blockchain model for cross-border data privacy protection is proposed to avoid the cross-border transmission of sensitive data through identity authentication. The model combines the SM2 and SM9 algorithms and blockchain technology to guarantee the security of stored data while providing a method to avoid sensitive data crossing borders and realizing cross-border identity authentication.

**Application Scenario:**
- Non-Fungible Token (NFT) project implementation
- Cross-border vehicle identity authentication
- IoV (Internet of Vehicles) applications
- State cryptographic algorithm integration

---

### 4.6 Research on the Mechanism of Privacy-Enhanced Cross-Institutional Data Sharing
**Authors:** (Authors to be confirmed - Springer)  
**Source:** Springer  
**Year:** 2024

This paper proposes a cross-institutional data sharing mechanism based on federated learning that achieves distributed data training through a blockchain and federated learning framework, avoiding direct data transmission and centralized storage, thus enhancing model performance while ensuring data privacy.

---

### 4.7 Blockchain-Based Secure Communication of Internet of Things in Space-Air-Ground Integrated Network
**Authors:** (Authors to be confirmed - Future Generation Computer Systems)  
**Source:** Future Generation Computer Systems  
**Year:** 2024

The paper introduces a decentralized data transmission framework that combines the characteristics of SAGIN and blockchain, leveraging the increasing computational and communication capabilities of low Earth orbit satellites. Simulation results show that the proposed scheme has excellent performance in terms of latency and throughput while ensuring the security of data transmission.

---

## 5. Specialized Document Security Solutions

### 5.1 A Survey of Blockchain-Based Privacy Applications
**Authors:** (Authors to be confirmed - arXiv Preprint)  
**Source:** arXiv  
**Year:** 2024

When blockchain technology is used for privacy-sensitive applications, it is crucial to analyze the privacy protections, consensus correctness, and auditability, with applications needing to integrate privacy protections within and outside the blockchain.

**Application Domains:**
- Consent management frameworks
- Self-sovereign identity (SSI) approaches
- Educational record management
- Active Assisted Living technologies
- Industrial IoT device identity

---

### 5.2 This Blockchain Solution is Changing Document Security and Certification
**Authors:** (Industry Case Study - KaliCertif)  
**Source:** Cointelegraph (KaliCertif Case Study)  
**Year:** 2024

KaliCertif, a blockchain-based platform, offers secure and easy-to-verify digital certificates for various documents and products, where once a certificate is generated, it is permanently recorded on the blockchain, providing a transparent and unalterable history. The platform utilizes NFC technology which enables wireless communication between devices over short distances to ensure proper certification of high-value products and artworks.

**Industry Collaborations:**
- Transportation companies for container traceability
- Universities for diploma certification
- High-value artwork authentication
- Integration through API for business workflows

---

### 5.3 Blockcerts - Blockchain Digital Document Verification System
**Authors:** (Technical/Industry Paper - PixelPlex)  
**Source:** PixelPlex

The system creates a decentralized blockchain ledger that uses strong cryptography, with enhanced safety and security of critical assets and procedures ensured by the smart contract suite embedded in the system that automates, tracks and logs every transaction. When a transaction occurs and all parties agree to the details, information is encoded into a block of digital data which is connected to adjacent blocks, creating an irreversible, immutable chain.

---

### 5.4 A Novel Architecture for Tamper Proof Electronic Health Record Management System using Blockchain Wrapper
**Authors:** (Authors to be confirmed - ACM Conference Paper)  
**Source:** ACM Proceedings - International Symposium on Blockchain and Secure Critical Infrastructure  
**Year:** 2019

This paper presents a comprehensive blockchain wrapper architecture ensuring tamper-proof electronic health record management with integration capabilities for existing healthcare IT systems.

---

### 5.5 A Blockchain-Based Framework for Electronic Medical Records Sharing with Fine-Grained Access Control
**Authors:** Jin Sun, Lili Ren, Shangping Wang, Xiaomin Yao  
**Source:** PLOS ONE  
**Year:** 2020

This distributed electronic medical records searchable scheme leverages blockchain and smart contract technology. The paper encrypts electronic medical data and stores it in the InterPlanetary File System (IPFS), a distributed storage protocol. The encrypted keyword index information is stored on the Ethereum blockchain, and a smart contract is used to realize keyword search. The scheme uses attribute-based encryption to ensure only authorized parties can decrypt EMRs.

**Key Features:**
- CP-ABE for fine-grained access control
- IPFS integration for distributed storage
- Smart contract-based keyword search
- Doctor-centric access control policy

---

### 5.6 Electronic Health Records Sharing Based on Consortium Blockchain
**Authors:** Guangfu Wu, Haiping Wang, Zi Yang, Daojing He, Sammy Chan  
**Source:** Journal of Medical Systems  
**Year:** 2024

This paper addresses medical data sharing using consortium blockchain with practical Byzantine fault tolerance consensus mechanism and proxy re-encryption techniques for secure cross-institutional data exchange.

---

### 5.7 Blockchain-Based Secure Storage Scheme for Medical Information
**Authors:** Zhijie Sun, Dezhi Han, and others  
**Source:** EURASIP Journal on Wireless Communications and Networking  
**Year:** 2022

This research combines IPFS and blockchain technology with attribute-based access control (ABAC) model for managing medical information. The paper addresses tamper protection and uses Ethereum blockchain with smart contracts for access control and data obfuscation, employing cryptographic methods for enhanced security.

---

## 5. Additional Recent Papers

### 5.8 Decentralized Secure Storage of Medical Records Using Blockchain and IPFS
**Authors:** R. Kumar, N. Marchang, R. Tripathi  
**Source:** Security and Privacy (Wiley)  
**Year:** 2021

This paper presents a comparative analysis of blockchain and IPFS-based healthcare secure storage solutions, examining how these technologies address the challenges of data loss, corruption, and ransomware attacks that plague traditional centralized storage systems.

--- ensuring tamper-proof electronic health record management with integration capabilities for existing healthcare IT systems.

---

## Key Themes and Findings

### Security Features
1. **Immutability**: All solutions leverage blockchain's inherent immutability to prevent document tampering
2. **Decentralization**: Elimination of single points of failure and central authority dependencies
3. **Cryptographic Security**: Integration of advanced encryption techniques (AES, RSA, ABE, proxy re-encryption)
4. **Transparency**: Audit trails and transaction history for accountability

### Technical Approaches
1. **Smart Contracts**: Automated access control and permission management
2. **Hash Functions**: Document fingerprinting and integrity verification
3. **Distributed Storage**: Integration with IPFS and cloud storage solutions
4. **Consensus Mechanisms**: DPoS, PBFT, and hybrid approaches for validation

### Application Domains
1. **Healthcare**: Electronic Medical Records, Personal Health Records, inter-hospital data sharing
2. **Legal**: Contract management, notarization, intellectual property protection
3. **Government**: Public records, identity verification, land registry
4. **General Document Management**: File sharing, cloud storage, certification

### Challenges Identified
1. **Scalability**: Transaction throughput and storage capacity limitations
2. **Performance**: Latency in consensus mechanisms and data retrieval
3. **Regulatory Compliance**: Legal frameworks and data privacy regulations (HIPAA, GDPR)
4. **Interoperability**: Integration with existing systems and cross-platform compatibility
5. **Cost**: Infrastructure and operational expenses

### Future Research Directions
1. Optimization of consensus algorithms for better performance
2. Integration with emerging technologies (AI, IoT, 5G/6G)
3. Enhanced privacy-preserving techniques (zero-knowledge proofs, homomorphic encryption)
4. Standardization of blockchain protocols for document management
5. User experience improvements and interface development

---

## Conclusion

The literature demonstrates significant research momentum in applying blockchain technology to secure document transmission and storage. Healthcare and legal domains show the most mature implementations, while government applications and cross-border data sharing represent emerging areas. The consistent themes across all papers emphasize blockchain's fundamental advantages: immutability, decentralization, transparency, and cryptographic security. However, practical deployment still faces challenges in scalability, regulatory compliance, and integration with legacy systems. Future research should focus on hybrid approaches that balance security, performance, and usability while addressing domain-specific requirements.

---

## References

All 20+ papers cited throughout this survey are referenced inline with appropriate citations. The papers span publications from 2018-2024 and include works from:
- IEEE Conference Proceedings
- ACM Digital Library
- Springer Nature journals
- PMC/NCBI medical databases
- ScienceDirect
- Scientific Reports
- Healthcare Technology Letters
- arXiv preprints
- Industry technical blogs and whitepapers