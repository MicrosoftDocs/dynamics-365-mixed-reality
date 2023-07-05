---
title: Electronic records and electronic signatures
description: Learn about the use of electronic records and signatures when you implement Dynamics 365 Guides in a regulated industry.
ms.date: 03/21/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Electronic records and electronic signatures

When you implement Dynamics 365 Guides in a regulated company, electronic records and electronic signatures are required (to a greater or lesser extent) to ensure traceability and compliance with regulatory requirements.

For example, [21 CFR Part 11](https://www.accessdata.fda.gov/scripts/cdrh/cfdocs/cfcfr/CFRSearch.cfm?CFRPart=11) is a section of the Code of Federal Regulations (CFR) that lays out the United States Food and Drug Administration's (FDA's) regulation about the use of electronic records and electronic signatures in the life science industry. It defines the criteria that determine whether electronic records and electronic signatures are accurate, authentic, trustworthy, reliable, confidential, and equivalent to paper records and handwritten signatures.

The following table summarizes 21 CFR Part 11.

| Area | Definitions |
|---|---|
| Scope | 21 CFR Part 11 applies to all electronic records that are created, modified, maintained, archived, retrieved, or transmitted under FDA regulation (predicate rules). |
| Electronic record management | <p>Computer system validation requires:</p><ul><li>System-enforced workflow sequencing.</li><li>Accurate, complete record accessibility throughout the record retention period.</li></ul> |
| Audit trail | <ul><li>The audit trail must include:<ul><li>A computer-generated date and time stamp for all changes.</li><li>Identification of the operator/signing person.</li><li>The purpose of the signature.</li></ul></li><li>The audit trail must be available throughout the record retention period.</li></ul> |
| Security | <ul><li>Role-based access control must be implemented to prevent unauthorized access.</li><li>Guidelines must be in place for ID/password management, electronic signatures, and system documentation control.</li></ul> |
| Electronic signatures | <ul><li>Each electronic signature must be unique to one individual and must not be reusable.</li><li>Signature manifestation in human-readable form must use at least two distinct identification components, such as an ID and a password.</li><li>Before the electronic signature is used, its binding authority must be certified to the FDA.</li></ul> |

21 CFR Part 11 requirements apply as defined by FDA [predicate rules](https://www.fda.gov/regulatory-information/search-fda-guidance-documents/part-11-electronic-records-electronic-signatures-scope-and-application). The requirements for records and signatures must be met by companies that use digital systems to manage compliance-related processes and documentation.

21 CFR Part 11 applies to records that must be maintained under the applicable regulation requirements, including:

- Records that are maintained in electronic format instead of paper format.
- Records that aren't identified in FDA regulations but are submissions that the FDA accepts in electronic format.

## Electronic records

[Electronic records](https://www.accessdata.fda.gov/scripts/cdrh/cfdocs/cfcfr/CFRSearch.cfm?CFRPart=11&showFR=1&subpartNode=21:1.0.1.1.8.2) are data and information that are created, modified, archived, retrieved, and distributed by a computer system.

## Electronic signatures

An [electronic signature](https://www.accessdata.fda.gov/scripts/cdrh/cfdocs/cfcfr/CFRSearch.cfm?CFRPart=11&showFR=1&subpartNode=21:1.0.1.1.8.3) is a set of encrypted electronic data that accompanies or is associated with an electronic document. Its basic functions are to unequivocally identify the signer and to ensure the integrity of the information and data in the signed document.

The electronic signature guarantees:

- **Authenticity**: The person who signed is part of the document information.
- **Integrity**: After the document is signed, the records can't be modified.
- **Non-repudiation**: The person who electronically signed can't say it wasn't them.

## Digital signatures (other than digitized signatures)

Digital signatures are a type of electronically based signatures that have a higher level of security. To perform the digital signature, a user name and two keys must be used. One of the keys is public, and the other is private.

## Audit trails

Audit trails are journals or records of modifications that are made to electronic records, either by users or by processes that operate on a user's behalf. Data must be protected from unauthorized modification and destruction, to allow for detection and after-the-fact investigations of security violations.

Audit trails:

- Must be computer generated.
- Can't be modified by the individual who created them.
- Must indicate when the data (record) was first entered, and who entered it.
- Must indicate who made any changes, and when.

## Security

Access must be limited to authorized individuals. The FDA recommends that:

- Each user of the system has an individual account.
- The system is designed to limit the number of sign-in attempts and to record unauthorized sign-in attempts.
- Users can work only under their own user profiles, and those profiles have unique user IDs and individual passwords.
- Individuals are prevented from signing in to the system so that they can give another person access to the system.
- Passwords or other access keys can be changed only at established intervals.
- Users sign out of the system when they leave a workstation.
- Automatic protection is installed and is activated after short periods of inactivity, to prevent unauthorized data entry.

## Other supporting material about 21 CFR Part 11

- [Electronic Systems, Electronic Records, and Electronic Signatures in Clinical Investigations: Questions and Answers](https://www.fda.gov/regulatory-information/search-fda-guidance-documents/electronic-systems-electronic-records-and-electronic-signatures-clinical-investigations-questions) (Draft Guidance for Industry)
- [Part 11, Electronic Records; Electronic Signatures - Scope and Application](https://www.fda.gov/regulatory-information/search-fda-guidance-documents/part-11-electronic-records-electronic-signatures-scope-and-application) (Guidance for Industry)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
