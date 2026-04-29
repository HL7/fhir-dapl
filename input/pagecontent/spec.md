This section defines the specific requirements for systems wishing to conform to profiles and operations specified in this IG. 

### Context

This DAPL IG is a library and as such does not define any conformance requirements, but rather defines profiles which can be used by other IGs such as DARTS IG. So implementers of DARTS or any other IG that leverages profiles from DAPL IG will be conformant to this IG. 

#### Pre-reading
Before reading this formal specification, implementers should first be familiar with two other key portions of the specification:

* The [Use Cases](usecases.html) page provides the business context and use cases that use the profiles specified by this IG.

* The [Background](background.html) page provides information about the underlying specifications and indicates what portions of each should be reviewed in order to have the necessary foundation to understand the constraints and usage guidance described in this detailed specification.


#### Conventions

This implementation guide uses terminology and key words from [RFC 2119](https://datatracker.ietf.org/doc/html/rfc2119) to indicate conformance requirements.

#### Claiming Conformance 

Actors and systems asserting conformance to this IG will use the profiles defined by this IG to exchange de-identified or anonymized data. This is typically done by implementing the DARTS IG.

The following definition of MUST SUPPORT is to be used in the implementation of the requirements.


##### MUST SUPPORT Definition

* <span class="fhir-conformance">Systems SHALL be capable of populating data elements as specified by the profiles and returning the data elements are returned using the specified APIs in the capability statement.</span>

* <span class="fhir-conformance">Systems SHALL be capable of processing resource instances containing the MUST SUPPORT data elements without generating an error or causing the application to fail.</span>


* <span class="fhir-conformance">Systems SHOULD be capable of displaying the MUST SUPPORT data elements for human use or storing it for other purposes.</span>

* <span class="fhir-conformance">In situations where information on a particular data element is not present and the reason for absence is unknown, Systems SHALL NOT include the data elements in the resource instance returned in response to the API requests.</span>

* <span class="fhir-conformance">When accessing de-identified or anonymized data, Systems SHALL interpret missing data elements within resource instances returned from API requests as data that has been removed as part of the de-identification and anonymization process.</span>



#### Profiles

This specification makes significant use of [FHIR profiles]({{site.data.fhir.path}}profiling.html) and terminology artifacts to describe the content to be shared as data exchange workflows. The implementation guide is based on [FHIR R4]({{site.data.fhir.path}}) and profiles are listed for each interaction.

The full set of profiles defined in this implementation guide can be found by following the links on the [FHIR Artifacts](artifacts.html) page.


#### System Actors, Requirements and Capability Statements

This DAPL IG does not specify any capability statements or systems or actors as this is just a library and the implementers of other IGs such as DARTS IG will specify the actors and Capability Statements required. 
