# Third-Party Data Breach: GRC & Incident Response Case Study
## Overview

This project analyzes a real-world third-party data breach involving C-Track, a court filing system provided by Thomson Reuters to the Minnesota Judicial Branch.

The case study applies a Governance, Risk, and Compliance (GRC) approach to examine the incident, identify security risks, evaluate control gaps, and develop recommendations for incident response, third-party risk management, and remediation.

This project is an independent analytical exercise based on publicly reported information. Where public reporting does not establish the technical root cause or specific control failures, those issues are identified as unknowns rather than presented as confirmed facts.

## Project Objectives
- Analyze a real-world cybersecurity incident
- Identify and assess information security risks
- Develop a risk register and risk matrix
- Identify potential security control gaps
- Evaluate third-party/vendor security risks
- Develop incident response recommendations
- Recommend vendor remediation and enforcement procedures
- Apply GRC concepts to a real-world scenario

## Skills Demonstrated

GRC

- Risk identification
- Risk assessment
- Risk scoring
- Risk register development
- Control gap analysis
- Third-party risk management
- Compliance benchmarking
- Remediation planning

Security

- Access control
- Least privilege
- Security monitoring
- Alerting
- Incident detection
- Incident escalation
- Vendor security oversight

Incident Response

- Incident timeline development
- Identification of potentially affected information
- Detection and escalation procedures
- Incident containment considerations
- Vendor access termination
- Remediation and reassessment

## Case Background

In March 2026, an unauthorized party obtained certain files from C-Track, a court filing system provided by Thomson Reuters. C-Track discovered unauthorized activity involving certain files on June 30, 2026. The investigation determined that the unauthorized party had obtained the files earlier in March.

Potentially affected information included individuals' names and, in some cases, Social Security numbers, driver's license numbers, dates of birth, medical information, and health insurance information. Certain confidential, redacted, or sealed court information may also have been affected.

Officials stated that court documents such as orders and briefs were not included in the incident.

In response, the Minnesota Judicial Branch terminated Thomson Reuters' access to court electronic environments, audited accounts, consulted technology experts and state authorities, and reported the incident to law enforcement.

## Incident Timeline

| Date | Event | Status |
| --- | --- | --- |
| March 2026 | An unauthorized party obtained certain C-Track files. | Confirmed |
| June 30, 2026 | C-Track discovered unauthorized activity involving certain files. | Confirmed |
| After June 30, 2026 | The investigation identified potentially affected files and courts. | Confirmed |
| September 2, 2026 | FOX 9 publicly reported the incident. | Confirmed |
| Unknown | Initial method used to gain unauthorized access. | Unknown |
| Unknown | Exact date the unauthorized party first gained access. | Unknown |
| Unknown | Exact date unauthorized access was terminated. | Unknown from available reporting |

## Risk Assessment

The assessment identified three primary risks associated with the incident:

- R-01 — Unauthorized Third-Party Access
- R-02 — Delayed Detection
- R-03 — Insufficient Third-Party Security Oversight

### R-01 — Unauthorized Third-Party Access

Risk Statement

There is a risk that unauthorized parties could access sensitive personal and court-related information through third-party vendor access if appropriate security controls are not implemented and maintained.

Likelihood: 4 — Likely

Unauthorized access could occur if appropriate security controls are not implemented and maintained, particularly where third-party vendors have access to sensitive information.

Impact: 5 — Severe/Critical

Sensitive information could be obtained and used for identity theft, while the initial compromise could also lead to additional sensitive information being exposed.

Risk Score: 20 — High/Critical

### R-02 — Delayed Detection

Risk Statement

There is a risk that delayed detection of unauthorized activity could allow an attacker to access additional sensitive information before the incident is identified and contained.

Likelihood: 4 — Likely

Delayed detection could occur again if appropriate security controls for monitoring, alerting, and incident detection are not established and maintained.

Impact: 5 — Severe/Critical

Delayed detection could allow unauthorized parties additional time to access or compromise critical and sensitive information, potentially increasing the scope and severity of the incident.

Risk Score: 20 — High/Critical

### R-03 — Insufficient Third-Party Security Oversight

Risk Statement

There is a risk that weaknesses in a third-party vendor's security controls could go unidentified if the organization does not regularly assess, monitor, and enforce vendor security requirements.

Likelihood: 4 — Likely

It is likely that a third-party vendor's security weakness could go unidentified if the organization does not regularly assess and monitor the vendor's security requirements.

Impact: 5 — Severe/Critical

Failure to identify a vendor's security weakness could allow a significant security incident to occur or remain undetected, potentially exposing sensitive information and causing serious operational, financial, legal, and reputational consequences.

Risk Score: 20 — High/Critical

## NIST 2.0 CSF Alignment
This assessment uses the NIST Cybersecurity Framework (CSF) 2.0 to organize the identified risks, control gaps, and recommended security practices.

| Project Area | NIST CSF 2.0 Alignment |
|---|---|
| Risk Assessment | ID.RA — Risk Assessment |
| Access Control | PR.AA-05 — Access permissions, entitlements, and authorizations |
| Security Monitoring | DE.CM — Continuous Monitoring |
| Third-Party Risk Management | GV.SC-05, GV.SC-06, GV.SC-07 — Cybersecurity supply chain risk management |
| Incident Response | RS.MA, RS.AN, RS.MI — Incident management, analysis, and mitigation |
| Recovery | RC.RP — Incident Recovery Plan Execution |

## Control Gaps

The identified risks indicate several security areas that should be evaluated.

### R-01 — Access Control

Control Gap

The company may not have sufficient access controls to ensure that only authorized users and third-party vendors can access sensitive information.

Controls to Evaluate

- Enforce least-privilege access
- Require unique user identification
- Log and monitor sensitive file access and transfers
- Require approval for privileged or third-party access
- Restrict vendors to information necessary for their contractual responsibilities

Recommended Response

The organization should implement least-privilege access, unique user identification, access logging, and approval requirements for privileged and third-party access.

### R-02 — Security Monitoring and Alerting

Control Gap

The company may not have sufficient security monitoring and alerting controls to detect suspicious activity quickly.

Controls to Evaluate

Security alerts for suspicious activity
Continuous security monitoring
Defined personnel responsible for investigating alerts
Escalation procedures for potential incidents
Documentation of investigation and response activities

Recommended Response

The organization should establish and maintain continuous security monitoring, automated alerts, and an escalation process that identifies who is responsible for investigating and confirming suspicious activity as a potential security incident.

Suggested Process

Detect → Alert → Investigate → Confirm → Escalate/Respond

The CISO or designated security personnel should investigate suspicious activity. A Data Protection Officer (DPO) should be involved when personal or regulated information is potentially affected.

### R-03 — Third-Party Risk Management

Control Gap

The company may not have sufficient security standards and assessment processes to ensure that third-party vendors maintain adequate security practices.

Controls to Evaluate

- Vendors must maintain security practices aligned with organizational security standards.
- Vendors should undergo periodic security assessments.
- Assessment results should be compared against established security requirements.
- Identified deficiencies should be documented and remediated.

Recommended Response

The organization should establish clear vendor security standards, conduct periodic security assessments, benchmark vendor compliance against those standards, require remediation of identified deficiencies within two weeks, and terminate vendor services when deficiencies remain unresolved after subsequent review.

## Recommended Incident Response
1. Detect

Identify suspicious activity through continuous security monitoring, automated alerts, and logging.

2. Investigate

Security personnel should investigate the alert to determine whether unauthorized activity occurred and identify potentially affected systems, accounts, and information.

3. Contain

Immediately restrict or terminate unauthorized access and, where appropriate, suspend third-party access while the investigation is conducted.

4. Remediate

Address the identified security weaknesses, reassess affected controls, and verify that remediation is effective before restoring or continuing access.

## Vendor Remediation & Enforcement

Third-party vendors should be held accountable for maintaining required security standards.

The proposed remediation process is:

Set Standards → Assess → Identify Gaps → Remediate → Reassess → Enforce

Vendors that fail a security assessment must remediate identified deficiencies within two weeks. Following a subsequent review, vendors with unresolved deficiencies will have their access and services terminated.

## Risk Register

The risk register is provided in the accompanying Excel workbook. It documents the identified risks, likelihood and impact ratings, risk scores, control gaps, recommended responses, and corresponding NIST CSF 2.0 alignment.

[View the Risk Register](./riskregister.xls)

## Lessons Learned

This incident demonstrates the importance of managing the security risks associated with third-party vendor relationships. While vendor partnerships can provide valuable services and capabilities, they can also introduce significant security risks when appropriate controls are not implemented and maintained. Unauthorized access can result in the compromise of sensitive information and cause operational and reputational damage.

This case also reinforced the importance of continuous security monitoring and alerting. Organizations should be able to identify suspicious activity quickly and have a clearly defined escalation process that identifies the appropriate personnel responsible for investigating and confirming potential security incidents.

Finally, organizations should establish clear security requirements for third-party vendors and regularly assess their compliance with those requirements. Periodic security assessments, compliance benchmarking, and defined remediation requirements can help organizations identify and address vendor security weaknesses before they develop into significant incidents.

## Key Takeaway

This case demonstrates how a cybersecurity incident can be evaluated through a GRC framework:

Research → Risk Assessment → Control Gap Analysis → Security Recommendations → Incident Response → Remediation

The objective of this project is not simply to describe a data breach, but to demonstrate the process of identifying security risks and developing practical controls and remediation strategies in response to them.
