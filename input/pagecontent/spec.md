This section defines the specific requirements for systems wishing to conform to profiles and operations specified in this IG. 

### Context

This DAPL IG is a library and as such does not define any conformance requirements, but rather defines profiles which can be used by other IGs such as DARTS IG. So implementers of DARTS or any other IG that leverages profiles from DAPL IG will be conformant to this IG. 

#### Pre-reading
Before reading this formal specification, implementers should first be familiar with two other key portions of the specification:

* The [Use Cases](usecases.html) page provides the business context and use cases that use the profiles specified by this IG.

* The [Background](background.html) page provides information about the underlying specifications and indicates what portions of each should be reviewed in order to have the necessary foundation to understand the constraints and usage guidance described in this detailed specification.


#### Conventions

This implementation guide uses specific terminology to flag statements that have relevance for the evaluation of conformance with the guide:

* **SHALL** indicates requirements that must be met to be conformant with the specification.

* **SHOULD** indicates behaviors that are strongly recommended (and which may result in interoperability issues or sub-optimal behavior if not adhered to), but which do not, for this version of the specification, affect the determination of specification conformance.

* **MAY** describes optional behaviors that are free to consider but where the is no recommendation for or against adoption.


#### Claiming Conformance 

Actors and Systems asserting conformance to this implementation guide will use the profiles defined by this IG to exchange deidentified or anonymized data. This is typically done by implementing the DARTS IG. 

The following definition of MUST SUPPORT is to be used in the implementation of the requirements.

##### MUST SUPPORT Definition

* Systems SHALL be capable of populating data elements as specified by the profiles 
* Systems SHALL be capable of processing resource instances containing the MUST SUPPORT data elements without generating an error or causing the application to fail. 
* Systems SHOULD be capable of displaying the MUST SUPPORT data elements for human use or storing it for other purposes.
* Systems SHOULD not include any additional extensions or data elements that is not identified as MUST SUPPORT in the profiles, unless there is a valid reason. 
* In situations where information on a particular data element is not present and the reason for absence is unknown, Systems SHALL NOT include the data elements or DataAbsentReason extension in the resource instance unless explicitly required by the profile.


#### Profiles
This specification makes significant use of [FHIR profiles]({{site.data.fhir.path}}profiling.html) and terminology artifacts to describe the content to be shared as part of UDS+ workflows. The implementation guide is based on [FHIR R4]({{site.data.fhir.path}}) and profiles are listed for each interaction.

The full set of profiles defined in this implementation guide can be found by following the links on the [FHIR Artifacts](artifacts.html) page.


#### System Actors, Requirements and Capability Statements

This DAPL IG does not specify any Capability Statements or Systems or Actors as this is just a library and the implementers of other IGs such as DARTS IG will specify the actors and Capability Statements required. 
