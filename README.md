# Decentralized Directory: Enhancing Trust in Digital Transactions

The Decentralized Directory (DeDi) Protocol is envisioned as a global, interoperable specification for accessing public directories. It unifies access to public information published by registrars, regardless of the underlying technology or jurisdiction, providing a standardized, open-source protocol for real-time look-up of any public directory. This protocol defines directories as a specialized subset of electronic registries containing publicly available information about entities and things. These directories are maintained by Directory Owners, who could be public authorities or trusted semi-public or private entities. A few examples, directory of language codes, location (State & District) codes, companies, banks, courts, ..and so on.

The DeDi Protocol offers a standardized, open-source specification that can be integrated into existing or new systems. It aims to unify diverse implementations, ensuring interoperability and trust across the ecosystem.

## Introduction
Every day, millions (if not billions) of transactions are carried out, exchanging value worth trillions of dollars seamlessly across national borders. This massive scale of digital commerce is underpinned by a global trend towards secure, interoperable, and efficient digital systems.
These systems are increasingly vital in protecting sensitive information, enhancing public services, and fostering economic growth in the digital age.

The turn of the millennium saw many countries formalize laws governing digital signatures in electronic commerce and communications, propelling the global economy into a new era. This “flattened the world”, enabling unprecedented levels of connectivity and efficiency in transactions.

## The Role of Trust (or Public Registries) in Digital Transactions
Central to the growth of e-commerce and e-governance is the issue of trust in the digital environment. The future of these sectors hinges on the trust that transacting parties place in the security of transmissions and the integrity of the communicated content.

Creating trust in the digital environment involves assuring the transacting parties about the integrity and confidentiality of the content of documents along with authentication of the sending and receiving parties in a manner that ensures that both the parties cannot repudiate the transaction.

In our interconnected digital world, trust is established through public information maintained by custodians, registrars, and institutions of authority. Public directories are crucial across various sectors, including governance, commerce, banking, healthcare, and education. They serve as the backbone for verifying the authenticity of entities, ensuring that transactions are legitimate and secure.

Registrars, as a trusted authority, approve the membership of an entity through rigorous due diligence and attestations, and publish a directory listing. Imagine various directories that are used daily. Directory of registered companies, banks, universities, non-profit organizations, schools, post offices, hospitals, police stations, courts, business establishments, and so on. National and international economies rely on such directories, maintained by registrars, as a foundational layer of trust.

## The Evolution of Public Information Sharing
Over the years, we have seen various methods for sharing public information. They can be broadly classified as:
1. [Gen 1] Registrar publishes a list of valid members as a document (PDF/Spreadsheet) on their website. These are meant to be downloaded and used. Not suitable for real-time updates and machine readability.

2. [Gen 2] Registrar provides a portal to look up valid members using unique registration numbers. These portal might be updated more frequently (since they are connected with the registration system) but may not provide machine readable output for external systems

3. [Gen 3] Registrar offers an API to retrieve the list of valid members. These APIs provide real-time and machine readable response / output, yet there will be multitudes of API specifications (custom to each system) making it a herculean task for product/app builders. For example, the CCADB is a registrar of sorts that manages the list of CAs that are included in root stores.  This is as close to a public directory that is managed today.

Of course, not to forget “Yellow Pages” - that served as a public directory of companies, business, doctors, lawyers, and so on. 😃

These methods have enabled a thriving digital economy but come with significant shortcomings:
1. Manual curation of lists: Prone to errors and inefficiencies.
2. Outdated cache entries: Out-of-sync databases lead to potential fraud.
3. Redundant efforts: Repetitive work across relying parties.
4. Custom interfaces: Fragmentation in how registrars provide access to information.
5. Lack of best practices: Issues such as key rotation are often overlooked.

## Current Best Practices and Challenges
Digital certificates are fundamental to establishing trust in electronic transactions. They serve as a digital form of identification for entities and individuals, ensuring that the parties involved in a transaction are who they claim to be. Public Key Infrastructure (PKI), which underpins digital certificates, relies on a chain of trust involving Certificate Authorities (CAs), Registration Authorities (RAs), and Certificate Revocation Lists (CRLs).

### Practical Challenges in Using Public Registries
Despite the critical role that public registries play, they face several practical challenges:
1. Manual Curation of Sources of Truth: Many registries still rely on manual processes for maintaining and updating records, which are prone to errors and inefficiencies. This manual curation can lead to outdated information and discrepancies that undermine trust.
2. Lack of Real-Time Discovery Interface: One of the significant gaps in current systems is the absence of a unified, real-time discovery interface for public keys. Without this, verifying the authenticity of entities in real-time is challenging, leading to potential security risks.
3. Risks with Revocation Lists: Certificate Revocation Lists (CRLs) are essential for maintaining the integrity of digital certificates by revoking compromised or expired certificates. However, the process is often slow and lacks real-time updates, creating windows of vulnerability where revoked certificates might still be trusted erroneously.

### The need for Decentralized Directory Protocol
While secure digital signing and certification systems have been established, several key pieces of the puzzle remain missing in realizing the full potential of a digitally trusted economy. The current systems often require scraping documents and databases to find registered entities, lack efficient methods to notify updates in digital certificates and cryptographic keys, and struggle to maintain the integrity of public keys (tracking key changes) across multiple systems.

What if a decentralized directory protocol could unify access to public information published by registrars, regardless of the underlying technology or jurisdiction?

To address these issues and accelerate the pace of economic growth, we need a highly reliable, performant, secure, open, and decentralized system that implements DeDi Protocol. This system should serve as the foundational layer for public directories, listing registered entities, their public keys, and other relevant information.

## Introducing the DeDi Protocol
The Decentralized Directory (DeDi) Protocol is envisioned as a global, interoperable specification for accessing public directories. It unifies access to public information published by registrars, regardless of the underlying technology or jurisdiction, providing a standardized, open-source protocol for real-time look-up of any public directory. This protocol defines directories as a specialized subset of electronic registries containing publicly available information about entities and things. These directories are maintained by Directory Owners, who could be public authorities or trusted semi-public or private entities.

The DeDi Protocol offers a standardized, open-source specification that can be integrated into existing or new systems. It aims to unify diverse implementations, ensuring interoperability and trust across the ecosystem.

![dedi_explainer_v1 drawio](https://github.com/user-attachments/assets/65246e75-9f60-4be0-899e-62c1dfbc85e8)

Here’s an example of DeDi Protocol

### dedi://example.com/directory-id{/record-id}


- `dedi`: This is the top level scheme for proposed URI format
- `//example.com/`: This part follows the scheme and specifies the server or domain where the directory service resides. Here, "example.com" is a placeholder, and the actual domain would depend on the specific service.
- `directory-id/`: This portion likely represents the identifier for a specific directory within the service. It could be a fixed name or dynamically generated depending on the implementation.
-  `{record-id}`: This part enclosed in curly braces {} is a placeholder for the actual record identifier within the directory.It's likely replaced with a specific ID when referencing a particular record.


### Key Benefits of DeDi:
1. Open-Source Protocol Specifications: Accessible to all, enabling widespread adoption and innovation.
2. Unified Access: Makes public information available irrespective of underlying technology. Ensuring compatibility with existing systems and technologies to promote widespread adoption.
3. Real-Time Discovery: Facilitates real-time look-up of public keys, ensuring the most current information is always available.
4. Community-Led Development: Ensures continuous improvement and relevance to the needs of the digital economy.
5. Enhanced Security: Reduces risks associated with outdated or compromised certificates by providing a standardized method for real-time updates.

In addition to this, a reference solution will also be made available for any organization to jump start their journey.

The Decentralized Directory Protocol is not a software solution or a prescriptive implementation guide; it is an enabler of trust in digital transactions. By implementing the DeDi Protocol, registrars and public authorities can maintain their directories in a verifiable, open, and trusted manner, driving innovation and trust in the digital economy.

This approach will open up new possibilities for market innovation, reduce inefficiencies, and ensure that the digital economy continues to thrive in a secure and trustworthy environment.

## Next Steps

The vision and technical details for Decentralized Directory are evolving. You can contribute and shape this along with the community by commenting/suggesting in [Decentralized Directory (DeDi) : A vision for public directories](https://docs.google.com/document/d/1pa16SrE29UjLhpOShnE5Wq1T_en_-4cQqmCbQ-X6WmQ/edit#heading=h.onjty42nibso)

Eventually, to realize the full potential of the Decentralized Directory Protocol, stakeholders are encouraged to:
1. Publish on public infrastructure offered through philanthropic efforts
2. Implement the DeDi standard in existing public registries to make them accessible
3. Adopt the DeDi Protocol to start looking up and querying public records in verification flows

Let’s co-create a future where trust is seamlessly integrated into every digital transaction.
