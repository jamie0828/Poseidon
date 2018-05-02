# Poseidon
Reform B2Bi/EDI with Block Chain Technology to build a trust business enviroment

## Goal
From technical aspect of view, the enterprise IT systems could be divided into two parts: Enterprise Internal system,such as ERP,CRM,HR and so on; And the data flow among enterprises(supply chain), normally it is called EDI(Electronic Data Interchange)/B2Bi(Business to Business Integration). The B2Bi is based on some protocols, such as AS2([https://en.wikipedia.org/wiki/AS2] Applicability Statement 2), OFTP([https://en.wikipedia.org/wiki/OFTP] Odette File Transfer Protocol),Rosettanet,etc.

This project try to build next generation of B2Bi protocol with last Block Chain technology to replace the current B2Bi protocols. The defects of current protocols will be overcome and the Block Chain benifit will be gained.

## Current B2Bi protocols
AS2 is the most polular protocol, so the the analysis below is based on AS2. AS2 have implements the blow features:
* Security
* Reliability
* Integrity
* None repudiation

Key technologies of AS2 are Asymmetric encryption,digital certificate,encryption/decryption, digital signature and MDN(Message Delivery Notification).

Althgouth AS2 is good and polular, it still has issues below

* **Architecture** AS2 is based on point to point communication, both sides need to be able to talk directly.　Once the receiver side is down or network is unsable, it does not work. From this point of view, the system is fragile. And broardcast mode is not supported.Once a big size data is sent to serveral partners, the performance become low.
* **Inconsistency** The data is stored at sender and receiver system, it still has the possible inconsistency especially the MDN is not returned successfully.
*  **Configuration** To configure AS2,  HTTP URL, digital certificate, etc. are prerequisites. It is impossible to work it out without an expert. 


## Design concept
The design can be logically seperated into two parts
**P2P network**  based communication with encryption transportation. A high availability network among all partners are established to exchanged business documents. The sender and receiver could be implemented with pulish/subscribe mode.

**Block chain** based data storage with decentral architecture to achieve data evidence.

## Challenge
* Performance and big data size
* Security consideration

## Implementation
A more detail draft specification will be worked out.
All advices and involvement are appericiate.
So far please reach me at jamie0828@163.com.

