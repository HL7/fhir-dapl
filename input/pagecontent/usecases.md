### Business Need and Use Cases

The section identifies the business needs and specific user stories for DAPL FHIR IG. Please refer to the Use Cases section of the DARTS IG for business need and use cases. The link is not here to avoid the circular dependency.

#### DAPL IG Profile Definitions and Conventions

This section clarifies the basic profile definitions specified in the IG and provides the context in which they need to be used.

##### Profiles common to De-identification and Anonymization

•	Many of the profiles that are defined in the IG are common to both de-identification and anonymization, such as profiles related to Diagnosis, Procedures, etc.

•	These profiles are named using the following convention: dapl-[Resource/Profile Name]. For example, for the Procedure resource, the name will be dapl-procedure, for the MedicationRequest resource, dapl-medicationrequest. 

* Profiles that don’t include the words "de-identified" or "anonymized" in the name can be used to represent both de-identified data and anonymized data.

When Profile Names are used.

•	Sometimes the IG uses a Profile name which is unique instead of a Resource name that is more general. For example, the IG uses lab-observation and income-observation where the Observation resource is profiled multiple times for different purposes. In these cases, the Profiles will be named like dapl-lab-observation.

Profiles used only to represent de-identified data.

•	Some profiles are to be used only to represent de-identified data which carry certain information about age, sex, race, ethnicities, or locations with a low risk of re-identification.

•	These profiles will be named as dapl-de-identified-[Resource/Profile Name] where, for example, the name would be dapl-de-identified-patient for the "Patient" Resource or dapl-de-identified-lab-observation for the “lab-observation” Profile.

Profiles used only to represent anonymized data.

•	Some profiles are to be used to represent only anonymized data that eliminates/generalizes age, sex, race, ethnicities, and locations further (beyond de-identified profiles) to eliminate re-identification risk.

•	These profiles will be named as dapl-anonymized-[Resource/Profile Name] where, for example, the name would be dapl-anonymized-patient for the "Patient" Resource.


### Identification Risk

The risk of identification when using the above profiles/data structures has to be ascertained by the healthcare organization releasing or providing the data based on the use case. The following are links that provide valuable industry regulations and guidance for risk assessments

* [HHS HIPAA De-identification Guidance](https://www.hhs.gov/hipaa/for-professionals/special-topics/de-identification/index.html) 
* [NIST Guidance](https://www.nist.gov/itl/iad/deidentification) 
* [NIST IR 8053 for De-identification](https://csrc.nist.gov/pubs/ir/8053/final)
