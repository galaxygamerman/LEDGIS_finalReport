## TL;DR

Blockchain research for secure document transmission and storage concentrates on hybrid on-chain/off-chain architectures, cryptographic access controls (CP-ABE, ABAC, searchable encryption), and IPFS or cloud-backed storage; measured advances show integrity, auditability, and fine-grained access but recurring gaps include privacy proofs, regulatory mapping, and large-scale deployments.

----

## Research landscape overview

This section situates the selected top 20 papers and summarizes their metadata and blockchain approaches to allow quick cross-reference. The table below lists each paper with authors, year, venue, and the primary blockchain implementation pattern reported in the paper.

| No. | Title and authors | Year | Venue | Blockchain approach | doi link |
|---|---|---:|---|---|---|
| 1 | Blockchain based searchable encryption for electronic health record sharing — Lanxiang Chen et al. | 2019 | Future Generation Computer Systems | Permissioned/consortium blockchain + searchable encryption and off‑chain EHR storage [1] | https://doi.org/10.1016/j.future.2019.01.018 |
| 2 | A secure and trustworthy medical record sharing scheme based on searchable encryption and blockchain — Xinyu Tang et al. | 2021 | Computer Networks | Blockchain + searchable encryption, smart‑contract access control, off‑chain storage [2] | https://doi.org/10.1016/j.comnet.2021.108540 |
| 3 | BPDS: privacy‑preserving data sharing for EMRs — Jingwei Liu et al. | 2018 | arXiv / Cryptography & Security | Consortium blockchain for indexes + cloud off‑chain storage, CP‑ABE access control, content extraction signatures [3] | https://doi.org/10.1109/GLOCOM.2018.8647713 |
| 4 | EduRSS: educational records secure storage and sharing — Hongzhi Li & Dezhi Han | 2019 | IEEE Access | Blockchain anchoring of off‑chain encrypted records, smart contracts for sharing and ACLs [4] | https://doi.org/10.1109/ACCESS.2019.2956157 |
| 5 | A secure data sharing platform using blockchain and IPFS — Muqaddas Naz et al. | 2019 | Sustainability | Ethereum smart contracts + IPFS, RSA/SSS encryption and role‑based access control [5] | https://doi.org/10.3390/su11247054 |
| 6 | Towards blockchain‑based secure storage and trusted data sharing for IoT — Z. Ullah et al. | 2022 | IEEE Access | Ethereum + IPFS, AES + ECDH, ABAC via smart contracts, PoA consensus tuning [6] | https://doi.org/10.1109/ACCESS.2022.3164081 |
| 7 | Secure data transmission of EHRs using blockchain — Rahul G. Sonkamble et al. | 2023 | Electronics | Hyperledger Fabric + IPFS, SPAKE key exchange, smart‑contract access control [7] | https://doi.org/10.3390/electronics12041015 |
| 8 | A blockchain based secure and privacy aware medical data sharing — S. Vidhya & V. Kalaivani | 2023 | Peer‑to‑peer Networking and Applications | Permissioned blockchain + smart contracts, LFC encryption, smart‑contract ACLs [8] | https://doi.org/10.1007/s12083-023-01449-1 |
| 9 | Secure document sharing model based on blockchain and ABE — Garima Verma & Soumen Kanrar | 2023 | Multimedia Tools and Applications | Blockchain + CP‑ABE/attribute‑based encryption and off‑chain storage [9] | https://doi.org/10.1007/s11042-023-16186-z |
| 10 | A Blockchain‑based Covert Document Communication System Model — Linru Ma | 2023 | ICCCS proceedings | Monero‑inspired structure + IPFS + attribute‑based encryption for covert transfer [10] | https://doi.org/10.1109/ICCCS57501.2023.10150544 |
| 11 | Towards securing digital documents using blockchain with off‑chain ABE — Shivani Pandey et al. | 2024 | IEEE (ETNCC) | On‑chain metadata + off‑chain storage + attribute‑based encryption (ABE) [11] | https://doi.org/10.1109/ETNCC63262.2024.10767571 |
| 12 | Security and Scalability of Blockchain Document Storage Systems — Sherwin Benjamin C et al. | 2024 | IEEE proceedings | Private Ethereum (PoA) + AES‑encrypted IPFS cluster + hashing on‑chain [12] | https://doi.org/10.1109/I-SMAC61858.2024.10714613 |
| 13 | hChain: Blockchain Based Large Scale EHR Data Sharing — Musharraf Alruwaill et al. | 2025 | arXiv preprint | Edge + IoMT integration, symmetric/asymmetric encryption, SHA‑256 hashing, smart contracts [13] | https://doi.org/10.48550/arXiv.2505.12610 |
| 14 | Efficient sensitivity orient blockchain encryption for cloud — A. Siva Kumar et al. | 2021 | Concurrent Engineering | Sensitivity‑aware blockchain encryption scheme (RSFSA) for cloud data [14] | https://doi.org/10.1177/1063293X211008586 |
| 15 | Secure and Efficient Data Storage and Sharing Scheme Based on Double Blockchain — L. Zhang et al. | (date n/a) | Tech Science / conference | Double‑blockchain architecture, ABE, encrypted EMR off‑chain storage [15] | https://doi.org/10.32604/cmc.2020.012205 |
| 16 | Method for storing and sharing secure files based on blockchain — Fan Kai et al. | 2018 | Patent | File pointers on blockchain, encrypted off‑chain files, PKC and ACLs recorded on ledger [16] |  |
| 17 | AES encryption in blockchain serverless storage — Meenakshi Kandpal et al. | 2024 | Facta universitatis | Permissioned blockchain + AES selected for serverless off‑chain encrypted storage [17] |  |
| 18 | Permissioned blockchain for automotive supply chain — Saima Zafar et al. | 2022 | Sensors | Hyperledger Fabric permissioned ledger for tamper‑proof records with practical evaluation [18] |  |
| 19 | Blockchain Tree for distributed personal ID data — Sergii Kushch et al. | 2019 | arXiv | Multilevel "Blockchain Tree" with subchains for ID data and access control [19] |  |
| 20 | Block Chain‑Based Secure Document Sharing — Sai Sandeep N & Magna Yadlapalli | 2025 | Indian J. of Computer Science & Technology | Ethereum + smart contracts + IPFS frontend/backend prototype and smart‑contract ACLs [20] |

Each table row is sourced from the cited paper and reflects the implementation choices and framing in that work [1] [2] [3] [4] [5] [6] [7] [8] [9] [10] [11] [12] [13] [14] [15] [16] [17] [18] [19] [20].

----

## Individual paper summaries

This section presents concise structured summaries of the 20 papers, emphasizing objectives, methods, main contributions, how each secures transmission/storage, and stated limitations. Each paper entry uses short labeled bullets for rapid scanning.

- **[1]**  
  - **Title authors year venue**: Blockchain based searchable encryption for electronic health record sharing — Lanxiang Chen et al., 2019, Future Generation Computer Systems [1].  
  - **Objectives and motivation**: Design a searchable‑encryption enabled blockchain EHR sharing system to give data owners control over access while enabling efficient searches across encrypted EHR indexes [1].  
  - **Methodology and blockchain implementation**: Uses a blockchain layer to record encrypted document indexes and smart contracts for access control; searchable encryption is combined with off‑chain EHR storage to enable privacy‑preserving searches [1].  
  - **Key findings and contributions**: Shows that blockchain anchoring plus searchable encryption provides owner control and searchable retrieval while preserving integrity and immutability of indexes [1].  
  - **Secure transmission and storage**: Original EHRs are stored off‑chain encrypted; blockchain stores tamper‑proof indexes/hashes and smart contracts mediate key release for secure retrieval [1].  
  - **Limitations mentioned**: Paper notes limited performance analysis at scale and lacks deployment/ regulatory discussion [1].

- **[2]**  
  - **Title authors year venue**: A secure and trustworthy medical record sharing scheme based on searchable encryption and blockchain — Xinyu Tang et al., 2021, Computer Networks [2].  
  - **Objectives and motivation**: Build a trustworthy EMR sharing scheme combining searchable encryption with blockchain assurances to support multi‑institution search and sharing [2].  
  - **Methodology and blockchain implementation**: Employs searchable symmetric encryption over off‑chain EMRs with blockchain storing encrypted indexes and smart contracts enforcing ACLs and transaction logic [2].  
  - **Key findings and contributions**: Demonstrates a scheme that allows cross‑institutional encrypted search and patient‑centric access control using smart contracts [2].  
  - **Secure transmission and storage**: EMRs remain encrypted off‑chain; the blockchain stores verifiable indexes and smart contracts handle secure key and access policy enforcement during transmission and retrieval [2].  
  - **Limitations mentioned**: Authors report limited performance benchmarking and note privacy extensions and compliance mapping are not fully explored [2].

- **[3]**  
  - **Title authors year venue**: BPDS: A blockchain based privacy‑preserving data sharing for electronic medical records — Jingwei Liu et al., 2018, arXiv [3].  
  - **Objectives and motivation**: Enable secure, privacy‑preserving EMR sharing across fragmented hospital systems while letting patients control sharing permissions [3].  
  - **Methodology and blockchain implementation**: Stores original EMRs encrypted in the cloud, reserves indexes on a consortium blockchain, and uses CP‑ABE for access control plus content extraction signatures for privacy [3].  
  - **Key findings and contributions**: Introduces BPDS combining consortium blockchain indexes with CP‑ABE to automate secure sharing and protect privacy via content extraction signatures [3].  
  - **Secure transmission and storage**: EMRs encrypted in cloud; blockchain ensures index immutability and smart contracts enforce patient‑defined access during transmission and retrieval [3].  
  - **Limitations mentioned**: Paper focuses on security analysis; it does not present large‑scale deployment metrics or regulatory discussion [3].

- **[4]**  
  - **Title authors year venue**: EduRSS: educational records secure storage and sharing — Hongzhi Li & Dezhi Han, 2019, IEEE Access [4].  
  - **Objectives and motivation**: Secure storage and sharing of digitized educational records while reducing computational cost versus CP‑ABE alternatives [4].  
  - **Methodology and blockchain implementation**: Off‑chain encrypted record storage with blockchains anchoring record hashes and smart contracts regulating sharing and verification [4].  
  - **Key findings and contributions**: Proof‑of‑concept and security analysis showing lower computational cost compared with CP‑ABE and MA‑CPABE while providing tamper‑evidence and sharing control [4].  
  - **Secure transmission and storage**: Original records remain encrypted off‑chain; on‑chain hashes allow recipients to verify integrity and smart contracts automate permissioned sharing [4].  
  - **Limitations mentioned**: Limited performance evaluation and no real‑world deployment or compliance mapping are provided [4].

- **[5]**  
  - **Title authors year venue**: A secure data sharing platform using blockchain and IPFS — Muqaddas Naz et al., 2019, Sustainability [5].  
  - **Objectives and motivation**: Replace trusted third parties for research/data marketplaces by combining blockchain and IPFS to deliver transparent, auditable sharing [5].  
  - **Methodology and blockchain implementation**: Uses Ethereum smart contracts, off‑chain IPFS storage, RSA authentication, Shamir Secret Sharing (SSS) for secret splitting, and incentive mechanisms via smart contracts [5].  
  - **Key findings and contributions**: Implements prototype with gas‑cost analysis and shows SSS outperforms AES variants in computational time in their evaluation [5].  
  - **Secure transmission and storage**: Files are encrypted/off‑chain on IPFS; content identifiers and access roles are enforced via smart contracts to ensure integrity and controlled retrieval [5].  
  - **Limitations mentioned**: Scalability beyond prototype, deeper privacy analyses, and deployment case studies are not addressed [5].

- **[6]**  
  - **Title authors year venue**: Towards blockchain‑based secure storage and trusted data sharing scheme for IoT environment — Z. Ullah et al., 2022, IEEE Access [6].  
  - **Objectives and motivation**: Secure IoT data storage/sharing without TPA, providing end‑to‑end encryption and fine‑grained access for resource‑constrained IoT scenarios [6].  
  - **Methodology and blockchain implementation**: Combines Ethereum smart contracts + IPFS, AES encryption, ECDH key exchange, ABAC policies in smart contracts, and replaces PoW with PoA for cost and throughput [6].  
  - **Key findings and contributions**: Demonstrates a practical, cost‑effective test‑net implementation (Rinkeby) and argues economic feasibility for IoT data [6].  
  - **Secure transmission and storage**: Data encrypted with AES; keys exchanged via ECDH; IPFS stores ciphertext while on‑chain records and ABAC smart contracts handle access control and auditability [6].  
  - **Limitations mentioned**: Lacks formal privacy proofs and long‑term deployment experiences; regulatory discussion absent [6].

- **[7]**  
  - **Title authors year venue**: Secure data transmission of electronic health records using blockchain technology — Rahul G. Sonkamble et al., 2023, Electronics [7].  
  - **Objectives and motivation**: Provide a patient‑centered PCHDM to improve confidentiality, access control, and privacy of EHRs [7].  
  - **Methodology and blockchain implementation**: Hyperledger Fabric private/permissioned network with IPFS off‑chain storage and SPAKE password‑based key exchange plus smart contracts for access policies [7].  
  - **Key findings and contributions**: Empirical evaluation on dataset measuring block creation time, computational overhead with encryption key size, and upload/download times, highlighting patient‑centric control [7].  
  - **Secure transmission and storage**: SPAKE secures key exchange, EMRs encrypted and stored on IPFS, smart contracts mediate access and logging ensuring integrity and controlled transmission [7].  
  - **Limitations mentioned**: Paper omits regulatory mapping and large‑scale real‑world deployment scenarios [7].

- **[8]**  
  - **Title authors year venue**: A blockchain based secure and privacy aware medical data sharing using smart contract and encryption scheme — S. Vidhya & V. Kalaivani, 2023, Peer‑to‑peer Networking and Applications [8].  
  - **Objectives and motivation**: Protect sensitive medical information with a permissioned blockchain plus cryptography and smart contracts [8].  
  - **Methodology and blockchain implementation**: Permissioned blockchain with smart contracts for ACLs and an LFC cryptographic algorithm securing records; authors describe immutability and access controls on‑chain [8].  
  - **Key findings and contributions**: Presents a design combining encryption and smart‑contract ACLs to guarantee confidentiality, integrity, and immutability of medical records [8].  
  - **Secure transmission and storage**: Records encrypted using LFC algorithm, access enforced via smart contracts; blockchain provides tamper‑evidence during transmission and storage [8].  
  - **Limitations mentioned**: Lacks performance metrics, advanced privacy techniques (e.g., ZKPs), and deployment case studies [8].

- **[9]**  
  - **Title authors year venue**: Secure document sharing model based on blockchain technology and attribute‑based encryption — Garima Verma & Soumen Kanrar, 2023, Multimedia Tools and Applications [9].  
  - **Objectives and motivation**: Provide strong confidentiality and fine‑grained access to documents combining blockchain and ABE [9].  
  - **Methodology and blockchain implementation**: Uses ABE for encryption and blockchain smart contracts to log and enforce access decisions; off‑chain storage is recommended for large files [9].  
  - **Key findings and contributions**: Demonstrates effective confidentiality and access control via ABEn + smart contracts and discusses efficiency benefits of off‑chain storage [9].  
  - **Secure transmission and storage**: Sensitive documents encrypted via ABE off‑chain; on‑chain metadata and smart contracts track permissions and transmission events [9].  
  - **Limitations mentioned**: Performance and scalability details are limited; regulatory and deployment aspects are not evaluated [9].

- **[10]**  
  - **Title authors year venue**: A Blockchain‑based Covert Document Communication System Model — Linru Ma, 2023, ICCCS proceedings [10].  
  - **Objectives and motivation**: Realize covert confidential document transmission that avoids attention in shared resource environments [10].  
  - **Methodology and blockchain implementation**: Combines Monero‑style privacy ideas, attribute‑based encryption, and IPFS for covert encrypted document transfer; experimental performance and concealment analysis are provided [10].  
  - **Key findings and contributions**: Proposes and experimentally validates a covert communication model that encrypts documents with ABE and uses IPFS for stealthy transfer [10].  
  - **Secure transmission and storage**: Documents encrypted with ABE, stored/transferred via IPFS; blockchain records access metadata to preserve traceability while aiming for concealment [10].  
  - **Limitations mentioned**: Focused on concealment and security proofs for the model; lacks compliance discussion and real‑world deployment evidence [10].

- **[11]**  
  - **Title authors year venue**: Towards Securing the Digital Document Using Blockchain with Off‑Chain ABE Framework — Shivani Pandey et al., 2024, IEEE ETNCC proceedings [11].  
  - **Objectives and motivation**: Strengthen digital document security by integrating off‑chain ABE with blockchain for traceable, efficient access control [11].  
  - **Methodology and blockchain implementation**: On‑chain metadata and audit trails, documents stored off‑chain and accessed after ABE‑based decryption when attributes satisfy policies [11].  
  - **Key findings and contributions**: Proposes a seven‑type document categorization and an off‑chain ABE governance architecture to improve throughput and user oversight [11].  
  - **Secure transmission and storage**: Off‑chain encrypted documents accessed via ABE; blockchain logs who accessed which documents and enforces policies [11].  
  - **Limitations mentioned**: Lacks detailed performance metrics, GDPR/HIPAA mapping, and deployment case studies [11].

- **[12]**  
  - **Title authors year venue**: Security and Scalability of Blockchain Document Storage Systems — Shyamala C et al., 2024, IEEE proceedings [12].  
  - **Objectives and motivation**: Investigate data security and scalability improvements in decentralized document storage using private Ethereum and IPFS clusters [12].  
  - **Methodology and blockchain implementation**: Private Geth node with PoA consensus, AES symmetric encryption for IPFS cluster storage, HTTPS for client communications, and hashing on‑chain for verification [12].  
  - **Key findings and contributions**: Describes an architecture demonstrating tamper‑evidence and discusses optimizations to improve performance in Ethereum + IPFS setups [12].  
  - **Secure transmission and storage**: Documents AES‑encrypted on IPFS‑cluster; blockchain stores hashes to allow validators to verify authenticity during retrieval and transmission [12].  
  - **Limitations mentioned**: Does not address privacy‑enhancing proofs, compliance, or broad deployment evidence [12].

- **[13]**  
  - **Title authors year venue**: hChain: Blockchain Based Large Scale EHR Data Sharing — Musharraf Alruwaill et al., 2025, arXiv preprint [13].  
  - **Objectives and motivation**: Combine IoMT edge resources with blockchain to enable real‑time secure EHR monitoring and sharing at scale [13].  
  - **Methodology and blockchain implementation**: Edge devices hash and encrypt data (symmetric/asymmetric), SHA‑256 for integrity, smart contracts for sharing; suggests location‑based authentication and edge pre‑processing [13].  
  - **Key findings and contributions**: Proposes hChain architecture to improve IoMT computing capacity and secure EHR sharing through smart contracts and edge‑assisted cryptography [13].  
  - **Secure transmission and storage**: Sensitive EHR data encrypted at edge; hashes anchored on blockchain to ensure immutability and smart contracts govern authorized transmissions [13].  
  - **Limitations mentioned**: Preprint highlights limited performance metrics, modest privacy mechanisms, and no compliance or deployment details [13].

- **[14]**  
  - **Title authors year venue**: Efficient sensitivity orient blockchain encryption for improved data security in cloud — A. Siva Kumar et al., 2021, Concurrent Engineering [14].  
  - **Objectives and motivation**: Introduce sensitivity‑aware blockchain encryption to better protect cloud‑hosted sensitive documents [14].  
  - **Methodology and blockchain implementation**: Proposes RSFSA sensitivity analysis integrated into blockchain encryption to prioritize protection for sensitive fields [14].  
  - **Key findings and contributions**: Presents a service‑centric sensitivity analysis approach combined with blockchain encryption to improve confidentiality for cloud documents [14].  
  - **Secure transmission and storage**: Sensitivity‑driven encryption controls which document parts are encrypted/stored and how keys are handled on‑chain to secure transmission and storage [14].  
  - **Limitations mentioned**: Paper lacks extensive deployment evidence, privacy proofs, and cross‑system performance benchmarks [14].

- **[15]**  
  - **Title authors year venue**: Secure and Efficient Data Storage and Sharing Scheme Based on Double Blockchain — L. Zhang et al. | date n/a | Tech Science |  
  - **Objectives and motivation**: Improve efficiency and security for EMR storage/sharing via a double‑blockchain architecture and ABE [15].  
  - **Methodology and blockchain implementation**: Uses a dual‑blockchain design to separate concerns (e.g., index vs. access logs), applies ABE for fine‑grained access and stores encrypted EMRs off‑chain [15].  
  - **Key findings and contributions**: Proposes the double‑blockchain model as a mechanism to balance security and efficiency in medical record sharing [15].  
  - **Secure transmission and storage**: Off‑chain encrypted EMRs plus on‑chain indexes and ACLs protect confidentiality during storage and transmission [15].  
  - **Limitations mentioned**: Paper provides limited detailed performance evaluation and lacks real‑world deployment data [15].

- **[16]**  
  - **Title authors year venue**: Method for storing and sharing secure files based on blockchain — Fan Kai et al., 2018, Patent [16].  
  - **Objectives and motivation**: Provide a practical method for encrypted file storage/sharing by recording pointers and access policies on blockchain [16].  
  - **Methodology and blockchain implementation**: Users encrypt/upload files, obtain file pointer; accounting nodes write access policy and pointer into blockchain account; key distribution after policy satisfaction [16].  
  - **Key findings and contributions**: Patent describes a ledger‑anchored pointer/ACL model ensuring availability and immutable access policy recording for file sharing [16].  
  - **Secure transmission and storage**: Encrypted files stored off‑chain; blockchain stores pointers and access policies; PKC is used for secure key exchange and policy enforcement during transmission [16].  
  - **Limitations mentioned**: Patent text does not present performance metrics or privacy‑enhancing proofs [16].

- **[17]**  
  - **Title authors year venue**: Towards data storage scheme in blockchain based serverless environment: AES approach — Meenakshi Kandpal et al., 2024, Facta universitatis [17].  
  - **Objectives and motivation**: Evaluate encryption algorithms for secure serverless blockchain storage and select the best fitted algorithm [17].  
  - **Methodology and blockchain implementation**: Evaluates Blowfish, RC4, DES, AES in a permissioned blockchain serverless framework and advocates AES for confidentiality and performance [17].  
  - **Key findings and contributions**: Recommends AES for permissioned blockchain storage in serverless contexts and outlines identity verification and permissioning mechanisms [17].  
  - **Secure transmission and storage**: AES encryption secures documents stored off‑chain; permissioned blockchain and identity verification control access and transmission [17].  
  - **Limitations mentioned**: Lacks wide performance benchmarking and detailed privacy/ compliance treatment [17].

- **[18]**  
  - **Title authors year venue**: Implementation of a distributed framework for permissioned blockchain‑based secure automotive supply chain management — Saima Zafar et al., 2022, Sensors [18].  
  - **Objectives and motivation**: Replace centralized tamperable vehicle records with a permissioned blockchain to secure automotive lifecycle data [18].  
  - **Methodology and blockchain implementation**: Hyperledger Fabric permissioned network implementation with custom chaincode; evaluation on memory, monetary cost, and record update speed [18].  
  - **Key findings and contributions**: Demonstrates practical memory and monetary costs and shows feasibility of permissioned blockchain for large user bases (reported memory estimate) [18].  
  - **Secure transmission and storage**: Uses permissioned blockchain to record hashes and transactions ensuring integrity; smart contracts govern record updates and transmissions between stakeholders [18].  
  - **Limitations mentioned**: Limited encryption detail and privacy‑preserving measures; regulatory analysis is absent though a practical case study is provided [18].

- **[19]**  
  - **Title authors year venue**: Blockchain Tree as Solution for Distributed Storage of Personal ID Data — Sergii Kushch et al., 2019, arXiv [19].  
  - **Objectives and motivation**: Propose a multilevel blockchain structure to increase security and access control for personal ID data [19].  
  - **Methodology and blockchain implementation**: Introduces "Blockchain Tree" with subchains integrated into higher‑level chains enabling hierarchical access control [19].  
  - **Key findings and contributions**: Suggests subchain architecture enhances security and multilevel access control for ID data management [19].  
  - **Secure transmission and storage**: Multilevel chains store ID data with access control embedded in subchains; tamper‑resistance and traceability are core features [19].  
  - **Limitations mentioned**: Encryption specifics, scalability benchmarks, and deployment evidence are not deeply addressed [19].

- **[20]**  
  - **Title authors year venue**: Block Chain‑Based Secure Document Sharing — Sai Sandeep N & Magna Yadlapalli, 2025, Indian Journal of Computer Science and Technology [20].  
  - **Objectives and motivation**: Build a practical decentralized document sharing system using Ethereum, IPFS and smart contracts to offer auditability and RBAC/ABAC [20].  
  - **Methodology and blockchain implementation**: Prototype using React/Web3 frontend, Express backend with (planned) IPFS integration, Ganache/Truffle local testing and Ethereum smart contracts for ownership/versioning and ACLs [20].  
  - **Key findings and contributions**: Demonstrates prototype features (tamper‑proof audit trail, attribute‑based access control) and discusses planned layer‑2 scalability solutions [20].  
  - **Secure transmission and storage**: Files encrypted before IPFS upload; contracts store content identifiers and enforce permissioned retrieval during transmission [20].  
  - **Limitations mentioned**: Integration challenges (IPFS), provider error handling, and production readiness remain outstanding; no wide deployment metrics [20].

----

## Themes methodologies and trends

This section synthesizes recurring themes, common methodologies, and implementation patterns observed across the surveyed papers, highlighting representative sources. The bullets below summarize cross‑paper trends and cite exemplar studies.

- **Blockchain plus off‑chain storage is dominant** — Many works place encrypted documents or full EMRs off‑chain (IPFS, cloud, IPFS‑cluster) while storing hashes, pointers, or indexes on‑chain to ensure integrity and reduce on‑chain storage costs [1] [3] [5] [6] [12].  
- **Attribute‑based and searchable encryption for fine‑grained access** — CP‑ABE/ABE and searchable encryption recur as mechanisms for expressive, patient/attribute‑based access control and private search over encrypted content [3] [1] [9] [11].  
- **Smart contracts implement access policies and audit trails** — Smart contracts are used as ACL engines and to automate sharing, purchases, or logging for auditability in many prototypes [5] [2] [20].  
- **Permissioned consortia and PoA for practical deployments** — Several implementations adopt permissioned ledgers (Hyperledger Fabric, private Ethereum with PoA) to meet throughput and governance requirements for enterprise/healthcare contexts [7] [12] [18].  
- **Symmetric/AES for bulk encryption; asymmetric/ECDH for key exchange** — Papers commonly use AES for encrypting large documents and asymmetric or key‑exchange protocols (ECDH, PKC) for secure key distribution noted across IoT/EHR solutions [6] [12] [17].  
- **Edge/IoMT and pre‑processing are emerging for scale** — Recent proposals incorporate edge hashing/encryption to reduce blockchain load and support IoMT real‑time scenarios [13].  
- **Evaluation focus varies from security proofs to gas/cost measures** — Some studies provide formal security analysis (BPDS), others include gas or latency benchmarking (Naz, Sonkamble), while many report limited performance evaluation [3] [5] [7].

For representative comparisons of methodologies used across papers see the table below.

| Methodology / pattern | Representative papers |  |
|---|---|  |
| IPFS + on‑chain hashes | [5] [6] [12] [20] |  |
| CP‑ABE / ABE | [3] [9] [11] |  |
| Searchable encryption | [1] [2] |  |
| Permissioned ledger (Hyperledger Fabric) | [7] [18] |  |
| AES bulk + asymmetric key exchange | [6] [12] [17] |

Each row references exemplar works that implement the pattern [5] [6] [12] [20] [3] [9] [11] [1] [2] [7] [18] [17].

----

## Research gaps and future directions

This section distills open research gaps reported across the corpus and proposes prioritized future directions grounded in the surveyed papers. The opening sentences tie observed shortcomings to opportunities for follow‑on work.

Across the surveyed literature, authors commonly report incomplete large‑scale evaluations, limited regulatory/compliance analysis, and few formal privacy proofs, pointing to concrete research opportunities. The bullets below list gaps and match them to supporting papers, followed by suggested future research directions.

- **Gaps identified**  
  - **Limited large‑scale performance and scalability evidence** — Multiple works note lack of stress tests, production deployments, or comprehensive throughput/latency studies [1] [2] [12] [20].  
  - **Sparse formal privacy proofs and advanced privacy mechanisms** — Few papers provide formal privacy models (e.g., differential privacy or ZKP integration) and many recommend stronger privacy analysis [3] [6] [8].  
  - **Regulatory and compliance mapping absent** — GDPR/HIPAA compliance considerations and data residency/regulatory mapping are generally not addressed [1] [11] [7].  
  - **Key management and revocation complexities underexplored** — Several designs use CP‑ABE or PKC but do not fully solve revocation, emergency access, or key‑rotation at scale [3] [9] [16].  
  - **Interoperability and standardization challenges** — Heterogeneous off‑chain storage and chain choices create integration concerns that are not standardized across systems [5] [12] [18].  
  - **Usability and real‑world governance** — User consent flows, multi‑stakeholder governance, and incentive design require more field studies [5] [20].

- **Future research directions**  
  - **Scalable hybrid architectures with benchmarks** — Design and publicly benchmark hybrid on‑chain/off‑chain frameworks under realistic workloads (document sizes, concurrency) following the architectures proposed in [12] [13] [6].  
  - **Formal privacy guarantees and ZKP integration** — Integrate succinct ZK proofs or privacy‑preserving searchable encryption and produce formal privacy/security proofs as recommended by [3] [6] [8].  
  - **Regulatory compliance frameworks and audits** — Map technical controls (encryption, audit trails) to legal requirements (HIPAA/GDPR) and evaluate governance models, as multiple papers flag missing regulatory discussion [1] [11] [7].  
  - **Key management, revocation, and emergency access primitives** — Advance revocation‑efficient ABE/CP‑ABE schemes or off‑chain revocation registries to address operational needs highlighted in [3] [9] [16].  
  - **Edge‑assisted pre‑processing and cost modeling** — Explore edge hashing/encryption and economic models to reduce on‑chain costs and latency for IoMT/EHR scenarios as suggested in [13] [6].  
  - **Interoperability standards and portability layers** — Specify metadata and pointer standards for on‑chain anchoring to enable cross‑system verification and portability across IPFS, cloud, and chains [5] [12].  
  - **Human factors and deployment studies** — Conduct user studies and pilot deployments for consent, usability, and governance to validate prototype claims in [20] [18] [5].

Each gap and recommendation is grounded in the surveyed papers that explicitly identify or imply the need for the change [1] [2] [3] [4] [5] [6] [7] [8] [9] [11] [12] [13] [16] [18] [20].

----