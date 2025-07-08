# smartgarden-legal
מדיניות פרטיות לAPI GPT
Privacy Policy – Smart Garden API
Last updated: July 8, 2025
(This document uses masculine and feminine pronouns interchangeably for convenience but is intended for all users.)

1. Who We Are
   Smart Garden API ("the Service," "we") provides a REST interface that enables:

* Weather forecasting for the GPS location of a garden
* Monthly planting calendar based on climate zone
* Image-based plant issue diagnosis

2. What Data We Collect
   \| Category           | Examples                            | Purpose of Processing                  |
   \|-------------------|-------------------------------------|----------------------------------------|
   \| Location Data      | Latitude/Longitude (lat, lon)       | Generating localized weather forecasts |
   \| Climate Zone Data  | Zone “9a”, “13b-IL”, etc.           | Creating relevant planting calendars   |
   \| Image Files        | Uploaded leaf/flower photo to /diagnose | Disease/pest analysis              |
   \| Technical Metadata | IP address, API client type, timestamp | Log monitoring, security, resource allocation |

We do not request or store names, emails, or payment details during the described API calls unless third-party OAuth modules are integrated by the operator.

3. Use of Information
   The collected data is used solely for:

* Responding to your API request – e.g., generating an accurate weather forecast
* Improving algorithm performance (anonymous statistics, such as diagnosis accuracy)
* Protecting against misuse (rate-limiting, attack detection)

4. Sharing and Disclosure with Third Parties

* No sale, rental, or publication of personally identifiable data
* Sub-processors (e.g., AWS S3, weather provider) receive only the minimum required to perform their service under data processing agreements
* Legal requirements – data will only be disclosed under a valid court order

5. Data Retention and Deletion
   \| Data Type           | Maximum Retention Period     | Deletion Mechanism                          |
   \|---------------------|------------------------------|---------------------------------------------|
   \| Log Data (IP, timestamp) | 30 days                   | Scheduled automatic deletion                |
   \| Image Files          | 24 hours                    | Encrypted at REST; manually deleted after diagnosis |
   \| Forecast/Planting Data | 14 days (in encrypted cache) | Expiration (TTL-based)                     |

API clients may send a DELETE /user-data request (if enabled) for immediate deletion of all identifiable stored items.

6. Security Measures

* HTTPS-only traffic
* AES-256 encryption for files at rest
* Key management via AWS KMS / Google Cloud KMS
* Least-privilege access control
* Quarterly code reviews and penetration testing

7. User Rights (GDPR/CCPA)
   You are entitled to:

* Access – receive a copy of the stored data (if applicable to your API key)
* Correction – request correction of errors
* Erasure/Right to be Forgotten – as outlined in Section 5
* Opt-out – object to processing for analytical/statistical purposes

For requests, see contact details in the section below.

8. Contact Information
   Smart Garden API – DPO
   Email: [privacy@smartgarden.io](mailto:privacy@smartgarden.io)
   Mail: 13 HaHaruv St., P.O. Box 456, Haifa 33045, Israel

9. Changes to This Policy
   We will update this document upon adding new features or regulatory changes. The updated date will appear at the top of this page. Continued use after changes implies agreement to the updated policy.
