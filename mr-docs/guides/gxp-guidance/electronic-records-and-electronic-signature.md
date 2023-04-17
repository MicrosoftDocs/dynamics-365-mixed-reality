---
title: Electronic records and electronic signature
description: Learn about the use of electronic records and signatures when implementing Dynamics 365 Guides in a regulated industry.
ms.date: 03/21/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Electronic records and electronic signature

When deploying Dynamics 365 Guides in a regulated company, electronic records and electronic signatures are required (to a greater or lesser extent) to ensure traceability and compliance with regulatory requirements.

For example, within life science, the United States Food and Drug Administration's (FDA) defines the electronic records and electronic signatures. [21 CFR Part 11](https://www.accessdata.fda.gov/scripts/cdrh/cfdocs/cfcfr/CFRSearch.cfm?CFRPart=11) is a section in the Code of Federal Regulations (CFR) that sets forth FDA's regulation on using electronic records and electronic signatures. It defines the criteria under which electronic records and electronic signatures are accurate, authentic, trustworthy, reliable, confidential, and equivalent to paper records and handwritten signatures.

This table summarizes the scope of Part 11.

| **Area** | **Definitions** |
|-------------------------|-------------------------|
| Scope | All electronic records created, modified, maintained, archived, retrieved, or transmitted under FDA regulation – predicate rules. |
| Electronic record management | Computer system validation requires: </br>- System-enforced workflow sequencing</br>- Accurate, complete record accessibility throughout the record retention period |
| Audit Trail | - Computer-generated date and time stamp for all changes, identification of operator/signing person, and purpose of the signature.</br> - Available throughout the record retention period. |
| Security | - Role based access control to prevent unauthorized access.</br>- Guidelines for ID/password management, electronic signatures, and system documentation control. |
| Electronic signatures | - Unique to one individual and not reusable.</br>- Signature manifestation in human readable form must use at least two distinct identification components, such as ID and password.</br>- Before use, must certify to FDA binding authority of electronic signature. |

21 CFR Part 11 requirements apply when defined by FDA [predicate rules](https://www.fda.gov/regulatory-information/search-fda-guidance-documents/part-11-electronic-records-electronic-signatures-scope-and-application). Records and signatures must be met by companies using digital systems to manage compliance-related processes and documentation. 21 CFR Part 11 applies to records required to be maintained under the applicable regulation requirements including:

- Records that are maintained in electronic format in place of paper format
- Records not identified in FDA regulations but are submissions the FDA accepts in electronic format

[**Electronic records**](https://www.accessdata.fda.gov/scripts/cdrh/cfdocs/cfcfr/CFRSearch.cfm?CFRPart=11&showFR=1&subpartNode=21:1.0.1.1.8.2) - Electronic records are data and information that are created, modified, archived, retrieved, and distributed by a computer system.

[**Electronic signature**](https://www.accessdata.fda.gov/scripts/cdrh/cfdocs/cfcfr/CFRSearch.cfm?CFRPart=11&showFR=1&subpartNode=21:1.0.1.1.8.3) - Electronic signature is a set of encrypted electronic data accompanying or are associated with an electronic document, whose basic functions are unequivocally identifying the signer and ensuring the integrity of the information and data contained in the signed document.

The electronic signature guarantees:

- Authenticity – the person who signed is part of the document information
- Integrity – after the document is signed, the records can't be modified
- Non-repudiation – the person who signed electronically cannot say it wasn't them

**Digital signatures** (other than digitized signatures) – Digital signatures are a type of electronically based signatures that have a higher level of security. To perform the digital signature, a username and two keys, public and private, must be used.

**Audit trail** – Audit trails are journals or records of modifications, by users or by processes operating on the user's behalf, to electronic-records. Data needs to be protected from unauthorized modification and destruction to enable detection and after-the-fact investigations of security violations. Audit trails:

- Must be computer generated
- Can't be modified by the individual who created them
- Must indicate when the data (record) was first entered and by whom
- Must indicate who made any changes and when

**Security** - Access must be limited to authorized individuals. The FDA recommends that:

- Each user of the system has an individual account.
- The system is designed to limit the number of log-in attempts and to record unauthorized access log-in attempts.
- Users can only work under their own user profiles encompassing unique user IDs and individual passwords.
- The system doesn't allow an individual to log into the system to provide another person access to the system.
- Passwords or other access keys can be changed only at established intervals.
- Users log off the system when leaving a workstation.
- An automatic protection is installed to activate after short periods of inactivity to avoid unauthorized data entry.

Other supporting material regarding 21 CFR Part 11:

- Use of Electronic Records and Electronic Signatures in Clinical Investigations Under 21 CFR Part 11 – [Questions and Answers: Draft Guidance for Industry](https://www.fda.gov/regulatory-information/search-fda-guidance-documents/electronic-systems-electronic-records-and-electronic-signatures-clinical-investigations-questions)
- Part 11, Electronic Records; Electronic Signatures - Scope and Application: [Guidance for Industry](https://www.fda.gov/regulatory-information/search-fda-guidance-documents/part-11-electronic-records-electronic-signatures-scope-and-application)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
