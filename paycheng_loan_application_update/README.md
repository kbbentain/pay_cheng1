# Paycheng Bank Loan Application Management System

## ServiceNow Update Set

This directory contains ServiceNow update set XML files for the Paycheng Bank Loan Application Management System.

## Scope
**x_1603889_paycheng**

## Structure

- `dictionary/` - Field definitions (sys_dictionary)
- `update/` - Table definitions, script includes, system properties, and other update records

## Components Included

### Tables
- `x_1603889_paycheng_loan_application` - Main loan application table

### Fields
All custom fields for loan applications including:
- Personal Information (Full Name, Contact, Email, Address, Birthdate)
- Employment Details (Employer, Job Position, Monthly Income, Years Employed)
- Loan Details (Loan Amount, Purpose, Term)
- Financial Information (Existing Loans, Monthly Expenses)
- AI Assessment (Credit Score, Risk Level, Assessment Notes)
- Document Management (Valid ID, Document Status, Rejection Reason)
- Officer Management (Assigned Officer, Decision, Comments)

### Choice Fields
- Loan Purpose (Home Improvement, Medical, Education, Business, Debt Consolidation, Other)
- Risk Level (Low, Medium, High)
- Application Status (Draft, Submitted, Under Review, Pending Documents, Approved, Rejected)
- Officer Decision (Approved, Rejected, Request Documents, Pending)
- Document Status (Not Verified, Valid, Invalid, Resubmission Required)

### Script Includes
- `PaychengAIScorer` - AI-powered credit scoring using Google Gemini API

### System Properties
- `x_1603889_paycheng.gemini_api_key` - Gemini API key for AI integration

## Installation

1. Import these XML files into ServiceNow Studio
2. Ensure the scope `x_1603889_paycheng` exists
3. The Gemini API key is pre-configured in the system property
4. Additional components (Business Rules, Client Scripts, UI Policies) should be created manually or imported separately

## Notes

- All XML files follow ServiceNow update set format
- Files are organized by type for easier management
- The Gemini API endpoint uses `gemini-2.0-flash` model

## Documentation

See the main README.md in the project root for complete implementation guide.

