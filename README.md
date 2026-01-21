# HL7 v2 – Remote Cardiac Monitoring Example

This repository contains a simple, end-to-end example of how HL7 v2 messages
are used in a hospital workflow.

The project follows a single outpatient cardiology case and focuses on how
patient data, clinical orders, and diagnostic results move between systems.

The goal is to understand HL7 through a concrete example rather than through
the specification alone.

---

## Clinical Scenario

A patient (Juana López) attends an outpatient cardiology visit due to
palpitations and dizziness.

Behind the scenes, hospital systems exchange information to:

1. Register the patient and create a visit  
2. Place a cardiac monitoring order (24-hour Holter)  
3. Return structured monitoring results  

---

## HL7 Messages Used

- **ADT^A01** – Patient registration and visit creation  
- **ORM^O01** – New order for ambulatory ECG (Holter)  
- **ORU^R01** – Structured monitoring results  

Each message builds on the previous one, keeping patient and order context
aligned across systems.


## Notes

This is a learning-focused project built to explore healthcare system
interoperability from a practical perspective.

The scope is intentionally limited to keep the example easy to follow.
