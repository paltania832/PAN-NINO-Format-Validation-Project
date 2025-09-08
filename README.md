# PAN-Number-Validation-Project

# Data Cleaning and Validation
# Objective
we are tasked with cleaning and validating a dataset containing the Permanent Account Numbers PAN of Indian nationals. The goal is to ensure that each PAN 
number adheres to the official format and is categorised as either Valid or Invalid. 
Dataset attached - PAN Number Validation Dataset.xlsx

 # Data Cleaning and Preprocessing:
1. Identify and handle missing data: PAN numbers may have missing values. These missing values need to be handled appropriately, either by removing rows or imputing values (depending on the context).
2. Check for duplicates: Ensure there are no duplicate PAN numbers. If duplicates exist, remove them. Handle leading/trailing spaces: PAN numbers may have extra spaces 
before or after the actual number. Remove any such spaces.
3. Correct letter case: Ensure that the PAN numbers are in uppercase letters (if any lowercase letters are present).

# PAN Format Validation: A valid PAN number follows the format:
1. It should be ten characters long.
2. The first five characters should be any upper case alphabets.
3. The next four-characters should be any number from 0 to 9.
4. The last(tenth) character should be any upper case alphabet.
5. It should not contain any white spaces.
 

1. Adjacent characters(alphabets) cannot be the same (like AABCD is invalid; AXBCD is valid)
   All five characters cannot form a sequence (like: ABCDE, BCDEF is invalid; ABCDX is valid)
2. The next four characters should be numeric (digits). Adjacent characters(digits) cannot be the same (like 1123 is invalid; 1923 is valid)
   All four characters cannot form a sequence (like: 1234, 2345
3. The last character should be alphabetic (uppercase letter).
 
 Example of a valid PAN: AHGVE1276F
 
 # Categorisation:
 Valid PAN: If the PAN number matches the above format.
 Invalid PAN: If the PAN number does not match the correct format, is incomplete, or contains any non-alphanumeric characters.
 
 # Tasks:
 Validate the PAN numbers based on the format mentioned above.
 Create two separate categories:
 Valid PAN
 Invalid PAN
 
 # Create a summary report that provides the following:
 1. Total records processed
 2. Total valid PANs
 3. Total invalid PANs
 4. Total missing or incomplete PANs (if applicable)

# NINO Format Validation Project
This project focuses on validating the National Insurance Number (NINO) format for individuals. 
# Key Features
1. NINO Format Validation
The validation logic checks that the NINO:
 - Does not start with banned prefixes: BG, GB, NK, KN, TN, NT, ZZ.
 - Has two letters at the start (excluding certain letters).
 - Is followed by six digits.
The validation ensures that each NINO is correctly structured before further processing.

2. Data Cleaning & Preprocessing
The project implements end-to-end data cleaning to prepare the dataset for accurate NINO validation:
- Handling missing values: Detects missing or null values in the dataset.
- Replacing NaN/Null with 'NA': Standardizes missing values for consistency.
- Removing missing values: Drops rows where NINO cannot be determined.
- Dropping duplicate records: Ensures each NINO appears only once.
- Uppercasing NINO values: Converts all NINO strings to uppercase to maintain uniformity.
  
3. Output

After processing, we need to export the below data to Excel File:
- Detailed NINO validation results: Each NINO is labeled as Valid or Invalid.
- Summary statistics: Total records processed, count of valid NINOs, and count of invalid NINOs.
