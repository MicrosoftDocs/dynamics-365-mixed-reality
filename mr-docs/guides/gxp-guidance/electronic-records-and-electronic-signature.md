---
title: 
description: 
ms.date: 03/09/2023
ms.topic: 
ms.service: 
author: 
ms.author: 
manager: 
---

#  Electronic records and electronic signature

When deploying Guides in a regulated company, electronic records and electronic signatures will usually be required (to a greater or lesser extent) to ensure traceability and comply with regulatory requirements.

For example, within life science, electronic records and electronic signature are defined by the United States Food and Drug Administration's (FDA). [21 CFR Part 11](https://www.accessdata.fda.gov/scripts/cdrh/cfdocs/cfcfr/CFRSearch.cfm?CFRPart=11) is a section in the Code of Federal Regulations (CFR) that sets forth FDA's regulation on using electronic records and electronic signatures. It defines the criteria under which electronic records and electronic signatures are accurate, authentic, trustworthy, reliable, confidential, and equivalent to paper records and handwritten signatures on paper.

The scope of Part 11 can be visually summarized by this table.

| **Area** | **Definitions** |
|-------------------------|-------------------------|
| Scope | All electronic records created, modified, maintained, archived, retrieved, or transmitted under FDA regulation – predicate rules. |
| Electronic record management | Computer system validation requires</br>system-enforced workflow sequencing, and</br>accurate, complete record accessibility throughout record retention period. |
| Audit Trail | Computer-generated date and time stamp for all changes, identification of operator/signing person, and purpose of the signature.</br>Available throughout record retention period. |
| Security | Role based access control to prevent unauthorized access.</br>Guidelines for ID/password management, electronic signatures, and system documentation control |
| Electronic signatures | Unique to one individual and not reusable.</br>Signature manifestation in human readable form must use at least two distinct identification components, e.g., ID and Password.</br>Must certify to FDA binding authority of electronic signature prior to use. |


21 CFR Part 11 requirements apply when defined by FDA [predicate rules](https://www.fda.gov/regulatory-information/search-fda-guidance-documents/part-11-electronic-records-electronic-signatures-scope-and-application)<u>.</u> Records and signatures must be met by companies using digital systems to manage compliance-related processes and documentation. 21 CFR Part 11 applies to records required to be maintained under the applicable regulation requirements:

-   That are maintained in electronic format in place of paper format

-   Not specifically identified in FDA regulations but are submissions the FDA accepts in electronic format

[**Electronic records**](https://www.accessdata.fda.gov/scripts/cdrh/cfdocs/cfcfr/CFRSearch.cfm?CFRPart=11&showFR=1&subpartNode=21:1.0.1.1.8.2) - Electronic records are data and information that are created, modified, archived, retrieved, and distributed by a computer system.

[**Electronic signature**](https://www.accessdata.fda.gov/scripts/cdrh/cfdocs/cfcfr/CFRSearch.cfm?CFRPart=11&showFR=1&subpartNode=21:1.0.1.1.8.3) - Electronic signature is a set of encrypted electronic data accompanying or are associated with an electronic document, whose basic functions are unequivocally identifying the signer and ensuring the integrity of the information and data contained in the signed document.

The electronic signature guarantees:

-   Authenticity – the person who signed is part of the document information

-   Integrity – after the document is signed, the records can't be modified

-   Non-repudiation – the persons who signed electronically cannot say it wasn't them

**Digital signatures** (other than digitized signatures) – Digital signatures are a type of electronically based signatures that have a higher level of security. To perform the digital signature, a username and two keys, public and private, must be used.

**Audit trail** – Audit trails are journals or records of modifications—by users or by processes operating on the user's behalf—to electronic-records. Data needs to be protected from unauthorized modification and destruction to enable detection and after-the-fact investigations of security violations.

Audit trails:

-   Must be computer generated

-   Can't be modified by the individual who created them

-   Must indicate when the data (record) was first entered and by whom

-   Must indicate who made any changes and when

**Security** - Access must be limited to authorized individuals. The FDA recommends that:

-   Each user of the system has an individual account

-   The system is designed to limit the number of log-in attempts and to record unauthorized access log-in attempts

-   Users can only work under their own user profiles encompassing unique user IDs and individual passwords

-   The system doesn't allow an individual to log into the system to provide another person access to the system

-   Passwords or other access keys can be changed only at established intervals

-   Users log off the system when leaving a workstation

-   An automatic protection is installed to activate after short periods of inactivity to avoid unauthorized data entry

You can find other supporting material/guides regarding 21 CFR Part 11 topic here:

-   Use of Electronic Records and Electronic Signatures in Clinical Investigations Under 21 CFR Part 11 – [Questions and Answers: Draft Guidance for Industry](https://www.fda.gov/regulatory-information/search-fda-guidance-documents/use-electronic-records-and-electronic-signatures-clinical-investigations-under-21-cfr-part-11)

-   Part 11, Electronic Records; Electronic Signatures - Scope and Application: [Guidance for Industry](https://www.fda.gov/regulatory-information/search-fda-guidance-documents/part-11-electronic-records-electronic-signatures-scope-and-application)

## Administration 

Your organization will need to focus on three administrative layers when implementing Guides in a regulated industry: HoloLens devices, the Power Platform (environments, Power Apps etc.), and software.  
  
These elements need to function independently as well as in conjunction with each other for Guides to run seamlessly. Otherwise, you risk malfunction which is critical from a product and a compliance perspective.

Overall, it is recommended to conduct a risk assessment to identify critical updates to devices, environments, and software. Based on the risk assessment, your organization should define if and where specific controls are needed to have devices, Power Platform components, and software in control.  
  
The following sections links to common tasks you perform to set up and maintain HoloLens devices and Power Platform environments. However, be aware that this is not an exhaustive user manual.


