This section provides an overview of the Implementation Guide (IG).

### IG Purpose

The purpose of this IG is to define a set of profiles that can be used to represent de-identified and anonymized information using FHIR profiles. The de-identified profiles and anonymized profiles are used for use cases such as 

* Health centers reporting to Federal agencies 
* Health centers releasing data for research


Read the Use Cases section of the DARTS IG to get an idea of the various systems, actors and the data flow requirements. 

### Guiding Principles for the IG

The following are the guiding principles for the DAPL IG.

* Define profiles that will enable data submitters to create de-identified/anonymized information using data present in the form of US Core or base FHIR resources. 
  
* Align with existing standards and regulations (e.g., ONC 2015 Edition, 2015 Edition Cures Update, HTI-1, HTI-4), United States Core Data for Interoperability (USCDI) while improving the timeliness and completeness of data for the specified [Use Cases](usecases.html).
 

### IG In-Scope Requirements

The following requirements are in-scope for the DAPL IG based on the use cases.

* Define the set of profiles that can be used to represent de-identified data
* Define the set of profiles that can be used to represent anonymized data

### IG Out-of-Scope 

The following aspects are out-of-scope for the DAPL IG based on the use cases.

* Risk Assessment on the profiles prior to exchanging data with the profiles 

* Policies and processes followed by Data Submitters which allow data sharing, collecting of consent, or compliance with regulatory requirements.

* Mechanisms to identify the patients for whom the data needs to be de-identified or anonymized


### Underlying Specifications

This guide is based on the [HL7 FHIR R4]({{site.data.fhir.path}}index.html) standard, and is aligned with [US Core IG]({{site.data.fhir.uscoreR4}}/index.html) terminology.

Implementers of the DAPL IG must understand basic information about the underlying specifications listed above.

