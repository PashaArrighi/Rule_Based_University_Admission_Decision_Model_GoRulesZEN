# Rule_Based_University_Admission_Decision_Model_GoRulesZEN

This project implements an **automated university admission decision process** using the **GoRules ZEN platform**. The goal is to simulate how institutions can assess applicants fairly and efficiently through predefined eligibility rules and transparent scoring.

## Overview
The model evaluates applicants based on four core attributes:
- **GPA**
- **Annual Income**
- **School Type**
- **Extracurricular Involvement**

Applicants receive a weighted score across these categories, and their **final admission status** is classified as:
- **Accepted** – Total Score ≥ 20
- **Backup** – Total Score between 15 and 19
- **Rejected** – Total Score < 15

## Workflow Logic
1. **Input Validation** – Ensures all required fields are provided and correctly formatted.
2. **GPA Eligibility Check** – Applicants with GPA below 3.0 are rejected.
3. **Scoring System** – Assigns points for:
   - **Annual Income** (≤ 40k: 10 pts, 40k–80k: 5 pts, > 80k: 2 pts)
   - **School Type** (Public: 10 pts, Private: 5 pts, Other: 0 pts)
   - **Extracurriculars** (Community Service: 10 pts, Sports/Music: 5 pts, None: 0 pts)
4. **Final Classification** – Total score determines admission result.

## Technology & Tools
- **Platform**: [GoRules ZEN](https://gorules.io)
- **Decision Logic**: JSON-based flow with function nodes, switch nodes, and validation steps.
- **Specification Document**: Includes business rules, test cases, and expected outputs.

## Test Cases
Example scenarios to verify model accuracy:
- **Accepted** – High score from all attributes.
- **Backup** – Moderate score (e.g., 15 pts).
- **Rejected** – Low GPA or missing data.
- **Edge Cases** – GPA exactly at 3.0, borderline scores.

## Purpose
- Demonstrates how **rule-based decision automation** can improve efficiency and fairness in admissions.
- Showcases **transparent, auditable scoring** that can be adapted for different institutions.
- Aligns with global best practices from **UNESCO, OECD, and World Bank** on AI in education.

## 📂 Repository Contents
- `JDM_Graph.json` – Decision model logic file for GoRules.

---
**Author**: Muhammad Pasha Arrighi Effendi  
