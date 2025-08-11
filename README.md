Dataset Composition:
The dataset includes resumes matched with job descriptions, with the assessment and scoring details based on various matching criteria:
- 201 Mismatched JSONs: Resumes that are not relevant to the provided JD.
- 648 Matched JSONs: Resumes that are relevant and aligned with the JD.


Dataset Structure:
Each sample JSON file in the dataset includes the following keys:

input:

job_description: Contains the full job description text.
macro_dict: A dictionary with macro-level criteria and their respective weighting.
micro_dict: A dictionary with micro-level criteria and their respective weighting.
additional_info: Extra requirements or preferences related to the JD.
minimum_requirements: List of fundamental qualifications for the role.
resume: Text of the resume as provided.
output:

justification: Reasons for the scores assigned, based on specific criteria.
scores:
macro_scores: Scores for broader criteria (e.g., experience, strategic thinking).
micro_scores: Scores for detailed criteria (e.g., market research expertise).
requirements: Boolean indicators showing if key requirements are met.
aggregated_scores: Overall scores for macro and micro criteria.
personal_info: Extracted personal details (e.g., name, contact details, current position).
valid_resume_and_jd: Boolean indicating if both resume and JD are valid for evaluation.
details:

Resume Analysis: Detailed breakdown of education, certifications, skills, project history, and professional experience.
