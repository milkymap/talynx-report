# CV Analysis Methodology

## Objective
To systematically and objectively identify the top candidates for a machine learning & image processing role based on the comprehensive analysis of 48 submitted CVs.

## Step 1: Data Extraction
- **Tools**: `pdftotext` (CLI)
- All CVs were provided in PDF format and converted to text using `pdftotext` for reliable, scriptable analysis.

## Step 2: Automated Keyword-Based Screening
- Each CV’s raw text was analyzed for critical keywords/themes linked to the hiring needs:
  - "machine learning", "deep learning", "computer vision", "image processing"
  - Key ML and CV libraries (e.g., TensorFlow, PyTorch, OpenCV, Keras)
  - Neural network terms (e.g., CNN, YOLO, segmentation, object detection, classification)
  - Evidence of significant experience (5+ years, PhD/Doctorate, or advanced academic background)
- For broad coverage, both English and French patterns were considered.

## Step 3: Scoring Criteria
The following points were assigned for each relevant occurrence or evidence:
- **Machine Learning**: 3 pts
- **Computer Vision**: 4 pts
- **Image Processing**: 3 pts
- **Deep Learning**: 3 pts
- **TensorFlow / PyTorch**: 3 pts
- **OpenCV**: 3 pts
- **CNN / Convolutional**: 2 pts
- **YOLO / Object Detection / Classification**: 3 pts
- **PhD / Doctorate**: 2 pts
- **Python + years / >= 5+ Years Experience**: 1 pt

CVs exceeding a **6-point threshold** were flagged for manual shortlist review.

## Step 4: Human Review and Candidate Ranking
- All high scoring CVs (≥6 pts) were manually checked for context, specific project accomplishments, and overall relevance.
- Special attention was paid to:
    - Depth and breadth of real ML/CV project delivery
    - Proven deployment of solutions (productization, industrial/medical/embedded)
    - Variety and complexity of datasets and deployment environments
    - Education, publications, and evidence of fast learning
- The top 3 profiles were selected based on total score, impact of past work, and strong fit for the stated position. Profiles feature in-depth summaries, technical strengths, and personalized justification.

## Step 5: Documentation and Reporting
- All processing scripts, scoring routines, and markdown profile reports (including methodology and summary tables) have been uploaded to the GitHub repository (`talynx-report`).
- Markdown files were used for transparency, reproducibility, and presentation to stakeholders.

## Evaluation Tools Used
- **pdftotext**: CLI/Unix utility for PDF to plain text conversion
- **bash scripting**: For mass file processing, extraction, scoring, and data wrangling
- **grep, head, sort, paste**: Unix commands for efficient pattern detection and report generation
- **Markdown**: For clear, readable documentation of process and results


## Evaluation Framework
- **Objective**: Maximize fairness, transparency, and relevance to role requirements
- **Reproducibility**: Scripts can be rerun on future candidate pools
- **Transparency**: All scoring rules and filter keywords are fully listed
- **Balance**: Automated flagging + manual qualitative judgment for final selection

## Notes
No personal or sensitive data beyond what’s present in submitted CVs is stored or shared. The repository is open for review; anonymized data or script samples can be provided upon request.

---
For more information or methodology questions, contact the repository owner.