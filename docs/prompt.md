## DentalWRK is a network of dental clinics that wants to track visits of customers, including procedures or diagnoses and their ordering dental practitioner. They need a database…

## Goal: Create a database design in 4NF to support this requirement, connecting a customer, a clinic and a dental practitioner. Here are the attributes we need for each of the entities:

### Entity	Attribute	Assumptions
#### Customer	
- Name:	Mandatory First name and last name. Optional: Middle name and suffix (e.g. Jr.). 
- Gender:	Mandatory
- Birthdate:	Mandatory
- Insurance:	Optional (The name of the dental insurance. Can change between visits. We need to have the correct one on each visit for billing.)
#### Dental practitioner	
- Name: Mandatory: First name and last name. Optional: Middle name and suffix (e.g. Jr.). 
- Specialty: Mandatory (Dentist, Periodontist, or Orthodontist)
#### Clinic	
- Name: Mandatory
- Full Address: Mandatory (break the address for easier querying)
#### Billable Outcome
- Type: Mandatory. Diagnosis or procedure
- Code: Mandatory. Diagnosis or procedure code
- Description: Mandatory (Text containing the description of the diagnosis or the procedure)

## Constraints & Assumptions
1.	Design table(s) to hold a clinic. Break the Clinic address down to address line, city, state, country and zip code. What do you gain by breaking it?
2.	A clinic can have multiple dental practitioners working in it. 
3.	Each time a customer is treated by dental practitioners, it is considered a separate visit.
4.	The billable outcomes of a visit could be a diagnosis or procedure. There could be more than one billable outcome per visit or none

## SQL Queries (Test Cases)
•	Which customers visited a certain clinic on any given date?

•	Which customers were seen by a certain dental practitioner in a certain clinic on any given date?

•	Which health insurance was charged to a customer for a given visit?
