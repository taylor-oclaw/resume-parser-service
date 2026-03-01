# HireFlow360 Resume Parser Unit Test Plan

## 1. Overview
This document outlines the unit test plan for the HireFlow360 resume parser service, covering PDF, DOCX, TXT parsing, skill extraction accuracy, experience timeline parsing, education parsing, and edge cases.

## 2. Test Cases

### 2.1 Parsing Formats

#### 2.1.1 PDF Parsing
- **Test Case 1**: Parse a simple resume in PDF format
  - **Input**: `simple_resume.pdf`
  - **Expected Output**: Parsed data including name, email, skills, experience, and education.

- **Test Case 2**: Parse a complex resume with multiple sections in PDF format
  - **Input**: `complex_resume.pdf`
  - **Expected Output**: Accurate parsing of all sections including nested or merged text blocks.

#### 2.1.2 DOCX Parsing
- **Test Case 3**: Parse a simple resume in DOCX format
  - **Input**: `simple_resume.docx`
  - **Expected Output**: Parsed data including name, email, skills, experience, and education.

- **Test Case 4**: Parse a complex resume with multiple sections in DOCX format
  - **Input**: `complex_resume.docx`
  - **Expected Output**: Accurate parsing of all sections including styles and formatting.

#### 2.1.3 TXT Parsing
- **Test Case 5**: Parse a simple resume in TXT format
  - **Input**: `simple_resume.txt`
  - **Expected Output**: Parsed data including name, email, skills, experience, and education.

### 2.2 Skill Extraction Accuracy
- **Test Case 6**: Test skill extraction from a resume with clear skill statements
  - **Input**: `skills_clear.txt`
  - **Expected Output**: List of all identified skills.

- **Test Case 7**: Test skill extraction from a resume with vague skill statements
  - **Input**: `skills_vague.txt`
  - **Expected Output**: Partially extracted skills based on context and keyword matching.

### 2.3 Experience Timeline Parsing
- **Test Case 8**: Parse an experience timeline with clear date ranges
  - **Input**: `experience_clear.pdf`
  - **Expected Output**: Correctly parsed start and end dates for each job entry.

- **Test Case 9**: Parse an experience timeline with ambiguous date ranges
  - **Input**: `experience_ambiguous.docx`
  - **Expected Output**: Best guess parsing of start and end dates, with warnings or error messages for ambiguous data.

### 2.4 Education Parsing
- **Test Case 10**: Parse education details from a resume
  - **Input**: `education_details.txt`
  - **Expected Output**: Correctly parsed degree names, institutions, and graduation years.

### 2.5 Edge Cases
- **Test Case 11**: Handle empty files
  - **Input**: `empty_file.pdf`, `empty_file.docx`, `empty_file.txt`
  - **Expected Output**: Parser should handle gracefully without throwing errors, returning an empty or minimal data set.

- **Test Case 12**: Handle corrupted files
  - **Input**: `corrupted_pdf.pdf`, `corrupted_docx.docx`, `corrupted_txt.txt`
  - **Expected Output**: Parser should detect and report corruption issues gracefully.

- **Test Case 13**: Parse non-English resumes
  - **Input**: `resume_non_english.pdf` (e.g., French, Japanese)
  - **Expected Output**: Parsed data with support for different languages. Skills, experience, and education should be parsed based on language-specific patterns or translation capabilities.
