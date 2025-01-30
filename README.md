# Dental Procedure Codes: American (ADA CDT) and Canadian (CDA)

This repository contains JSON files for dental procedure codes used in the **United States (ADA CDT)** and **Canada (CDA)**. These files include procedure names, average times, and notes for common dental procedures. The data is structured in a standardized format for easy integration into applications, billing systems, or dental practice management software.

---

## Files in This Repository

1. **`ada_cdt_codes.json`**  
   - Contains dental procedure codes based on the **American Dental Association (ADA) Current Dental Terminology (CDT)**.  
   - Used in the United States for billing, insurance claims, and record-keeping.  

2. **`cda_codes.json`**  
   - Contains dental procedure codes based on the **Canadian Dental Association (CDA)** coding system.  
   - Used in Canada for billing, insurance claims, and record-keeping.  

---

## Structure of the JSON Files

Both files follow the same structure for consistency. Each procedure includes:  
- **`code_type`**: The category of the procedure (e.g., Examination, Restoration).  
- **`name`**: The name of the procedure.  
- **`time`**: The average time required for the procedure, broken into `min`, `max`, and `unit` (e.g., minutes).  
- **`notes`**: Additional details about the procedure.  

For multi-appointment procedures (e.g., crowns, dentures), the `time` field is broken into stages (e.g., preparation, try-in, delivery).

---

## Example: ADA CDT Code (United States)

```json
"D0120": {
  "code_type": "Examination",
  "name": "Periodic Oral Evaluation",
  "time": {
    "min": 15,
    "max": 20,
    "unit": "minutes"
  },
  "notes": "Established patient, routine evaluation"
}
