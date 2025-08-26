# Linux Department Data Automation

This repository contains Bash scripts to automate the creation of dummy company department data and back it up to a blob storage container.  
It was built to simulate departmental file structures and demonstrate automated backup workflows using Linux tools.

## Features
- Generates dummy files and folders for departments: HR, Finance, IT, Marketing, and Logs  
- Automatically organizes files into department-specific directories and subfolders  
- Creates CSVs, text files, and placeholders for typical company data  
- Automates zipping and uploading of department folders to a blob storage container using `azcopy`  
- Timestamped backups for easy tracking

## Scripts

### 1. Generate Dummy Company Data (`generate_company_data.sh`)
- Creates department folders under a base directory (default: `~/company_data`)  
- Populates each department with example files:
  - HR: employee lists, policies, recruitment notes  
  - Finance: budgets, payroll, invoices  
  - IT: network diagrams, software inventory, policies  
  - Marketing: campaigns, social media reports, graphics placeholders  
  - Logs: sample system logs  

**Usage**:
```bash
chmod +x generate_company_data.sh
./generate_company_data.sh
