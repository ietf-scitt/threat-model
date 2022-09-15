---

title: SCITT Threat Model and Security Considerations
abbrev: SCITT Threat Model
docname: draft-threat-model-latest
stand_alone: true
ipr: trust200902
area: Security
wg: TBD
kw: Internet-Draft
cat: std
consensus: yes
submissiontype: IETF
pi:
  toc: yes
  sortrefs: yes
  symrefs: yes
kramdown_options:
  auto_id_prefix: sec-

author:
- ins: Y. Deshpande
  name: Yogesh Deshpande
  organization: ARM
  street: 110 Fulbourn Road
  code: 'CB1 9NJ'
  city: Cambridge
  email: yogesh.deshpande@arm.com
  country: UK
- ins: A. Delignat-Lavaud
  name: Antoine Delignat-Lavaud
  organization: Microsoft Research
  street: 21 Station Road
  code: 'CB1 2FB'
  city: Cambridge
  email: antdl@microsoft.com
  country: UK
- ins: C. Fournet
  name: Cedric Fournet
  organization: Microsoft Research
  street: 21 Station Road
  code: 'CB1 2FB'
  city: Cambridge
  email: fournet@microsoft.com
  country: UK
normative:
venue:
  type: non-WG
  mail: scitt@ietf.org


--- abstract

SCITT Threat Model document does an extensive analysis of possible threats to SCITT building blocks and overall threats to the SCITT System. This document is to be read in tandem to the SCITT Architecture Document.

--- middle

# INTRODUCTION

This document provides the information about the threats that were considered for SCITT, and also discusses possible mitigation strategies. This will lead to defining the security requirements for the SCITT Architecture.

It also clearly defines certain threats that are out of scope of the SCITT.


# System Level Threats

* Denial of Service:

An attacker may flood any part of SCITT Eco System that prohibits correct users from using the system.

* Information Disclosure:

A third party may be able to extract sesitive information from SCITT Eco System, example either from SCITT append only log or from receipts that are confidential.

* Loss of Credentials:

An attacker may get access to the credentials of a specific actor and can perform its roles incorrectly. For example, a rogue actor getting access to auditor credentials and generating false audit reports for the SCITT Claims.


# Component Level Threats
The threats are categorized based on the individual building blocks that comprise the SCITT Architecture.

## Identity Threats

* False Identity

* Stolen Identity

## Threats to Transparency Service

* Refuse or delay registration of claims

* Register claims that do not pass its registration policy

* Issue verifiable receipts for claims that do not match its log

* Provide log access to only limited actors within a set of authorized actors

* Provide log access to unauthorized actors

* Presenting a forked view of log to only a sub-set of users

* Provide access to unrelated claims to authorized third parties

* Unauthorized access to policy documents, that control the behaviour of the log

## Threats to Independent Verifiers

* Compromised Verification Logic

* Usage of incorrect receipts during verification

# Out of Scope

The following threats does impact SCITT Eco System but they are covered by other WG, hence out of scope from SCITT perspective.

* SCITT append only logs running compromised Hardware, Firmware or Software
If the log operation is compromised due to any of th above been compromised, then Remote Attestation of the log servers, as defined in IETF RATS should address the same.

* Incorrect use of security practices

--- back

# Attic

Not ready to throw these texts into the trash bin yet.
