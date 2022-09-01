
# INTRODUCTION

This document provide the information about the threats that were considered for SCITT, and also discusses possible mitigation strategies. This will lead to defining the security requirements for the SCITT.

It also clearly defines certain threats that are out of scope of the SCITT.


# System Level Threats

* Denial of Service
An attacker may flood any part of SCITT Eco System that prohibits correct users from using the system.

* Information Disclosure
A third party may be able to extract sesitive information from SCITT Eco System, example either from SCITT append only log or from receipts that are confidential.

* Loss of Credentials
An attacker may get access to the credentials of a specific actor and peforming its roles incorrectly. For example, A rogue actor getting access to auditor credentials and generating false audit reports for the SCITT Claims.


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

* Provide access of log to unauthorized actors

* Presenting a forked view of logs to only a sub-set of users

* Provide access to unrelated claims to authorized third parties.

* Access to Policy documents, that control the behaviour of the log

## Threats to Independent Verifiers

* Compromised Verification Logic

* Usage of incorrect receipts during verification

# Out of Scope

The following threats does impact SCITT Eco System but they are covered by other WG, hence out of scope from SCITT perspective.

* SCITT append only logs running compromised Hardware, Firmware or Software
If the log operation is compromised due to any of th above been compromised, then Remote Attestation of the log servers, as defined in IETF RATS should address the same.

* Incorrect use of security practices

