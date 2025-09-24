 Clinic Booking System - Relational Database

Overview
This database models a clinic booking system where:
- Patients book appointments with doctors.
- Doctors belong to departments.
- Doctors prescribe medicines to patients during appointments.

The schema ensures **normalization** (up to 3NF), clear relationships, and proper constraints.

---

Database Schema

1. Department
Stores medical departments (e.g., Pediatrics, Cardiology).

2. Doctor
Doctors working in the clinic, linked to departments.

3. Patient
Patients registered in the clinic.

4. Appointment
Bookings between patients and doctors.

5. Medicine
Medicines available in the clinic.

 6. Prescription
Many-to-Many relationship between appointments and medicines.

---

 Relationships
- One-to-Many
  - Department → Doctor  
  - Patient → Appointment  
  - Doctor → Appointment  

- Many-to-Many
  - Appointment ↔ Medicine (via `Prescription`)  

---

Usage
1. Run the schema:
   ```sql
   
