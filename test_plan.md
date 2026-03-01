# HireFlow360 Resume Parser Test Plan

## Table of Contents
1. [Introduction](#introduction)
2. [Test Cases for PDF Parsing](#test-cases-for-pdf-parsing)
3. [Test Cases for DOCX Parsing](#test-cases-for-docx-parsing)
4. [Test Cases for TXT Parsing](#test-cases-for-txt-parsing)
5. [Skill Extraction Accuracy](#skill-extraction-accuracy)
6. [Experience Timeline Parsing](#experience-timeline-parsing)
7. [Education Parsing](#education-parsing)
8. [Edge Cases](#edge-cases)

## Introduction
The test plan is designed to ensure the HireFlow360 resume parser service accurately extracts and parses data from resumes in various formats including PDF, DOCX, TXT.

## Test Cases for PDF Parsing
- **Test Case 1: Basic PDF Parsing**
  - Input: A simple PDF resume with basic information.
  - Expected Output: All text is extracted without errors.
- **Test Case 2: Complex PDF Parsing**
  - Input: A complex PDF resume with multiple sections, graphics, and tables.
  - Expected Output: Relevant text is extracted accurately despite complexity.

## Test Cases for DOCX Parsing
- **Test Case 3: Basic DOCX Parsing**
  - Input: A simple DOCX resume with basic information.
  - Expected Output: All text is extracted without errors.
- **Test Case 4: Complex DOCX Parsing**
  - Input: A complex DOCX resume with multiple sections, graphics, and tables.
  - Expected Output: Relevant text is extracted accurately despite complexity.

## Test Cases for TXT Parsing
- **Test Case 5: Basic TXT Parsing**
  - Input: A simple TXT resume with basic information.
  - Expected Output: All text is extracted without errors.
- **Test Case 6: Complex TXT Parsing**
  - Input: A complex TXT resume with multiple sections and formatting.
  - Expected Output: Relevant text is extracted accurately despite complexity.

## Skill Extraction Accuracy
- **Test Case 7: Skill Extraction from PDF**
  - Input: A PDF resume containing a skills section with specific keywords.
  - Expected Output: All relevant skills are correctly identified and extracted.
- **Test Case 8: Skill Extraction from DOCX**
  - Input: A DOCX resume containing a skills section with specific keywords.
  - Expected Output: All relevant skills are correctly identified and extracted.
- **Test Case 9: Skill Extraction from TXT**
  - Input: A TXT resume containing a skills section with specific keywords.
  - Expected Output: All relevant skills are correctly identified and extracted.

## Experience Timeline Parsing
- **Test Case 10: Experience Parsing from PDF**
  - Input: A PDF resume containing an experience section with dates and roles.
  - Expected Output: Correct parsing of the start and end dates, as well as roles and responsibilities.
- **Test Case 11: Experience Parsing from DOCX**
  - Input: A DOCX resume containing an experience section with dates and roles.
  - Expected Output: Correct parsing of the start and end dates, as well as roles and responsibilities.
- **Test Case 12: Experience Parsing from TXT**
  - Input: A TXT resume containing an experience section with dates and roles.
  - Expected Output: Correct parsing of the start and end dates, as well as roles and responsibilities.

## Education Parsing
- **Test Case 13: Education Parsing from PDF**
  - Input: A PDF resume containing an education section with school names, dates, and degrees.
  - Expected Output: Accurate extraction of schools, graduation dates, and degrees earned.
- **Test Case 14: Education Parsing from DOCX**
  - Input: A DOCX resume containing an education section with school names, dates, and degrees.
  - Expected Output: Accurate extraction of schools, graduation dates, and degrees earned.
- **Test Case 15: Education Parsing from TXT**
  - Input: A TXT resume containing an education section with school names, dates, and degrees.
  - Expected Output: Accurate extraction of schools, graduation dates, and degrees earned.

## Edge Cases
- **Test Case 16: Empty File**
  - Input: An empty PDF, DOCX, or TXT file.
  - Expected Output: Parser should handle gracefully without errors.
- **Test Case 17: Corrupted File**
  - Input: A corrupted PDF, DOCX, or TXT file.
  - Expected Output: Parser should handle gracefully without errors.
- **Test Case 18: Non-English Resume**
  - Input: Resumes in different languages (e.g., Spanish, French).
  - Expected Output: Parser should extract readable text and attempt to identify skills, experience, and education with reasonable accuracy.