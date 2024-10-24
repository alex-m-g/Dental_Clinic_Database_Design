# Dental_Clinic_Database_Design

This repository contains the database design for **DentWiz**, a network of dental clinics that wants to track visits, procedures/diagnoses, and their associated dental practitioners.

## Project Structure

- **docs/**: Contains the prompt and project documentation.
- **sql/**: Contains the SQL script used to create the database schema, including tables, triggers, and relationships.
- **models/**: Contains the MySQL Workbench model (`.wmb`) for the database design.
- **LICENSE**: License information for the repository.

## Requirements

This project was designed based on the following requirements:

- Track dental visits with details about customers, clinics, and dental practitioners.
- Track billable outcomes of each visit (diagnosis or procedure).
- Record and store dental insurance information for billing, which may change between visits.

For full details, please see the [project prompt](docs/prompt.md).

## Design Preview
![github](https://github.com/user-attachments/assets/258cde6e-0c27-4a3c-8b08-2a1c82011375)


### Prerequisites

- [MySQL](https://www.mysql.com/) installed.
- [MySQL Workbench](https://www.mysql.com/products/workbench/) for visualizing the `.wmb` file.

### Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/alex-m-g/Dental_Clinic_Database_Design.git
   cd Dental_Clinic_Database_Design
