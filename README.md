# Resume Screening Agent (HR & Recruitment)

An automated screening pipeline agent that evaluates applicant text resumes against a targeted Job Description (JD) and generates an ordered ranking matrix based on criteria alignment.

---

## 📋 Challenge Deliverables Included
* **Job Description**: Handled inside `job_description.txt`
* **Folder of Sample Resumes**: Found in the `resumes/` directory folder
* **Ranked Output**: Structured evaluation layout saved at `ranked_candidates.json`
* **Scoring Method Note**: Detailed explanation provided below.

---

## 🛠️ Execution Instructions

1. Clone this repository locally:
   ```bash
   git clone https://github.com
   cd hr-recruitment-agent
   ```
2. Run the agent using python:
   ```bash
   python agent.py
   ```

---

## 🧠 Scoring Methodology & Architecture Tradeoffs

### Scoring System
* **Technical Skills Match (50%)**: Direct comparison of required keywords (e.g., Python, Git, SQL) against candidate proficiencies.
* **Professional Experience (50%)**: Verification of job timeline lengths against required seniority.

### Design Choices & Tradeoffs
* **File Architecture**: Chosen plain `.txt` inputs instead of native `.pdf` parsing libraries. This ensures immediate code compatibility and high execution speeds without environment setup failures during testing.
