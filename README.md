# OSINT-Based Threat Intelligence Assessment

## Cyber Threat Intelligence | OSINT | Digital Footprint Analysis | Threat Assessment

### Project Overview

This project presents a **passive, OSINT-based Cyber Threat Intelligence (CTI) assessment** of **VFS Global**, an international organisation providing visa, passport, and consular services.

The assessment was conducted to identify publicly observable security risks associated with the organisation's digital footprint, with particular attention to:

* Phishing and brand-impersonation threats
* Publicly exposed domains, hosts, and infrastructure
* Potential data-leakage indicators
* Email and subdomain exposure
* Historical changes to the organisation's web presence
* Indicators that could potentially be leveraged by threat actors

The investigation used publicly available information and defensive intelligence techniques. **No exploitation, brute-force activity, unauthorized access, or intrusive testing was performed.**

---

## Objectives

The assessment was guided by three primary intelligence requirements:

1. **Are there phishing or brand-impersonation threats targeting VFS Global?**
2. **Are there publicly exposed assets that could potentially be leveraged by attackers?**
3. **Is the VFS Global brand being abused for fraudulent activity?**

These requirements were used to structure the OSINT collection and analysis process.

Full Project Report

View the Full OSINT Threat Intelligence Report- (OSINT-Based-Threat-Intelligence-Assessment.pdf)

## Methodology

The investigation followed a structured Cyber Threat Intelligence lifecycle:

Planning & Direction
        ↓
Collection
        ↓
Processing
        ↓
Analysis
        ↓
Dissemination
```

The methodology focused on passive OSINT collection and validation of publicly available information.

### Intelligence Collection

Information was collected through:

* Search-engine reconnaissance
* Google Dorking
* Email and subdomain enumeration
* Public breach-intelligence checks
* Domain and infrastructure reputation checks
* Historical web analysis
* Publicly available security intelligence sources

The report documented the discovery of **37 URLs, 161 IP addresses, 636 hosts, and one publicly identified email address** during the collection phase.

---

## Tools Used

| Tool                             | Purpose                                                                     |
| -------------------------------- | --------------------------------------------------------------------------- |
| **Google Search / Google Dorks** | Discovery of publicly indexed domains, pages, files and potential exposures |
| **theHarvester**                 | Passive email, host and subdomain enumeration                               |
| **Sublist3r**                    | Subdomain discovery                                                         |
| **VirusTotal**                   | Domain, URL and indicator reputation validation                             |
| **AbuseIPDB**                    | IP reputation analysis                                                      |
| **Wayback Machine**              | Historical website and infrastructure analysis                              |
| **Have I Been Pwned**            | Public breach-exposure checks                                               |
| **MXToolbox**                    | Email and domain security analysis                                          |

The report maps these tools to different stages of the OSINT investigation.

---

## Key Findings

### 1. Phishing & Brand Impersonation

The investigation identified multiple VFS Global-related URLs and country-specific subdomains.

Because VFS Global operates as a third-party service provider for governments and diplomatic missions, many country-specific subdomains were determined to be part of its legitimate digital footprint.

The investigation did **not identify confirmed phishing pages, cloned login pages, or high-confidence malicious look-alike domains** during the assessment period.

However, the number of country-specific domains represents an area that should continue to be monitored because threat actors could potentially exploit familiarity with the brand and legitimate-looking domain structures.

---

### 2. Infrastructure Exposure

The assessment identified publicly visible VFS Global services and infrastructure, including services associated with passport and visa tracking.

Examples documented in the assessment include:

```text
passport.vfsglobal.com
visatracking.vfsglobal.com
visa.vfsglobal.com
```

The investigation did not identify evidence of unauthorized exposure or significant infrastructure misconfiguration during the assessment period.

---

### 3. Data Leakage Indicators

Public breach-intelligence checks did not identify a confirmed breach associated with the email address examined during the investigation.

The report also found no confirmed exposed documents or leaked email credentials within the investigated public sources.

---

## Indicator Validation

The collected indicators were subjected to additional validation to reduce false positives.

### VirusTotal

The assessment recorded clean reputation results for the primary domain and selected subdomains, including:

vfsglobal.com             → 0/91 detections
visa.vfsglobal.com        → 0/92 detections
mohesr.vfsglobal.com      → 0/95 detections
```

### AbuseIPDB

The assessed IP addresses had **0% confidence of malicious activity / no previous reports** in the checks documented by the report.

### Have I Been Pwned

The publicly identified email address checked during the assessment returned **no breach exposure** in the source used for the investigation.

---

## Threat Actor Perspective

Although no immediate compromise was identified, the investigation highlighted the potential for threat actors to exploit the organisation's extensive country-specific digital footprint for:

* Brand impersonation
* Phishing campaigns
* Fraudulent visa-related services
* Credential harvesting
* Social engineering

The report therefore treats **brand impersonation and phishing infrastructure as ongoing monitoring requirements rather than confirmed incidents**.

---

## Business Risk

Potential consequences of a successful brand-impersonation or phishing campaign could include:

* Financial losses
* Fraud against customers
* Reputational damage
* Loss of customer trust
* Regulatory consequences
* Increased operational and incident-response costs

For an organisation involved in visa, passport and consular services, maintaining customer trust and protecting the integrity of its digital identity are particularly important.

---

## Recommendations

Based on the findings, the assessment recommends:

### Continuous Brand Monitoring

Monitor for:

* Typosquatting domains
* Look-alike domains
* Newly registered domains containing the organisation's name
* Suspicious certificates
* Fake login portals
* Fraudulent visa-service websites

### Infrastructure Monitoring

Establish recurring OSINT monitoring to identify newly exposed infrastructure and suspicious changes to the organisation's public digital footprint.

### Threat Intelligence Monitoring

Continue validating newly discovered indicators through reputation and breach-intelligence platforms.

### Credential Exposure Monitoring

Where legitimate credentials are confirmed to have appeared in breach intelligence, appropriate credential-rotation and incident-response procedures should be initiated.

### Recurring OSINT Sweeps

The assessment recommends recurring OSINT collection—such as weekly monitoring—to identify newly emerging phishing infrastructure at an early stage.

---

## Evidence & Investigation Log

The project maintained evidence throughout the investigation, including:

* OSINT collection results
* Discovered URLs
* IP addresses
* Hosts
* Email intelligence
* Historical website observations
* Reputation-validation results
* Breach-intelligence results

The original assessment records **161 IP addresses, 37 URLs, 636 hosts and one publicly identified email address** from the collection process.

---

## Skills Demonstrated

This project demonstrates practical experience in:

* Cyber Threat Intelligence
* Open-Source Intelligence (OSINT)
* Digital footprint analysis
* Attack-surface awareness
* Domain and subdomain enumeration
* Email intelligence
* Google Dorking
* Threat indicator validation
* IP reputation analysis
* Breach-intelligence analysis
* Historical web analysis
* Threat actor perspective analysis
* Risk assessment
* Security documentation
* Evidence collection
* Security recommendations
* Ethical cybersecurity research

---

## Ethical Considerations

This project was conducted strictly for **educational and defensive cybersecurity purposes**.

The investigation:

* Used publicly available information
* Did not attempt unauthorized access
* Did not exploit vulnerabilities
* Did not perform brute-force attacks
* Did not intentionally disrupt systems
* Did not access restricted information

The original report explicitly defines the engagement as passive OSINT and states that no exploitation was conducted.

---

## Project Deliverables

```text
OSINT-Based-Threat-Intelligence-Assessment/
│
├── README.md
│
├── report/
│   └── OSINT-Based-Threat-Intelligence-Assessment.pdf
│
├── evidence/
│   ├── screenshots/
│   └── tool-outputs/
│
├── indicators/
│   └── IOC-summary.md
│
└── references/
    └── sources.md
```

> --

## Project Outcome

The assessment found **no confirmed high-confidence compromise, phishing infrastructure, or significant public data exposure** within the investigated sources during the reporting period.

The principal security takeaway was that the organisation's extensive digital footprint and country-specific domains warrant **continuous brand-impersonation and OSINT monitoring**.

The project demonstrates how publicly available intelligence can be systematically collected, validated, analysed and transformed into actionable defensive security recommendations.

---

## References

The investigation referenced publicly available security and OSINT resources including:

* theHarvester
* Sublist3r
* VirusTotal
* AbuseIPDB
* Have I Been Pwned
* Google Search / Google Dorks
* Wayback Machine
* MXToolbox

---

## Author

**Oyebola Owolabi**

Cybersecurity Analyst in Training | Journalist | Performing Artist

**Project Date:** August 2026
