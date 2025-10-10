# Online Exam Proctoring Platform with AI - Project Documentation

## Project Information

**Title:** Online Exam Proctoring Platform with AI-Powered Real-Time Monitoring

**Student:** Humayun Ahmed
**Registration No:** 19502005005
**Session:** 2019-2020

**Supervisor:** Prof. Dr. Mohammed Shakhawat Hossain
**Institution:** Daffodil Institute of IT (DIIT)
**Affiliated with:** National University of Bangladesh

**Date of Submission:** January 16, 2025

---

## Project Overview

This project presents an AI-powered online exam proctoring platform that leverages advanced computer vision technologies (YOLOv8n and MediaPipe) to provide automated, real-time monitoring of examination sessions. The platform implements a dual-camera architecture using WebRTC technology with real-time alerts via Socket.IO (<150ms latency).

### Key Technologies

- **Frontend:** React.js v18+, Tailwind CSS
- **Backend:** Flask (Python 3.8+) RESTful API
- **Database:** MySQL 8.0+ (21 normalized tables)
- **AI Models:** YOLOv8n (object detection), MediaPipe (facial analysis)
- **Real-time Communication:** WebRTC, Socket.IO
- **Security:** JWT authentication, HTTPS/TLS, AES-256 encryption
- **Compliance:** GDPR, CCPA, FERPA

---

## Document Structure

### Chapters

1. **Chapter 1: Introduction** (5-6 pages)
   - Overview, Problem Statement, Motivation, Objectives, Scope, Limitations

2. **Chapter 2: Background Study** (9-10 pages)
   - Related Work, System Challenges, Feasibility Study, Research Gap
   - Includes 2 tables (Platform Comparison, Cost-Benefit Analysis)

3. **Chapter 3: System Design and Analysis** (13-15 pages)
   - 9 System Design Diagrams
   - Database Schema (21 entities, 3NF)
   - Includes 1 table (Technical Specifications)

4. **Chapter 4: Implementation Details** (Pending)

5. **Chapter 5: Results and Testing** (Pending)

6. **References** (IEEE format)

### Tables

- **Table 2.1:** Comparative Analysis of Commercial Proctoring Platforms
- **Table 2.2:** Cost-Benefit Analysis: Manual vs. AI-Powered Proctoring
- **Table 3.1:** System Architecture Technical Specifications

### Figures (9 Diagrams in Chapter 3)

| Figure | Diagram Type | File Location | Draw.io Source |
|--------|--------------|---------------|----------------|
| 3.1 | Flowchart | `Chap3/flowchart` | `3.2_Flowchart.drawio` |
| 3.2 | Workflow | `Chap3/workflow` | `3.3_Workflow_Diagram.drawio` |
| 3.3 | Use Case | `Chap3/usecase` | `3.4_Use_Case_Diagram.drawio` |
| 3.4 | Activity | `Chap3/activity` | `3.5_Activity_Diagram.drawio` |
| 3.5 | Sequence | `Chap3/sequence` | `3.6_Sequence_Diagram.drawio` |
| 3.6 | DFD Level 0 | `Chap3/dfd_level0` | `3.7_DFD_Level_0_1_2.drawio` (Tab 1) |
| 3.7 | DFD Level 1 | `Chap3/dfd_level1` | `3.7_DFD_Level_0_1_2.drawio` (Tab 2) |
| 3.8 | DFD Level 2 | `Chap3/dfd_level2` | `3.7_DFD_Level_0_1_2.drawio` (Tab 3) |
| 3.9 | ER Diagram | `Chap3/er_diagram` | `3.8_3.9_ER_Diagram.drawio` |

**Note:** Figures 3.6 & 3.7 are placed on the same page. Figures 3.8 & 3.9 are placed on the same page.

---

## Compilation Instructions

### Prerequisites

- LaTeX distribution (TeX Live, MiKTeX, or MacTeX)
- BibTeX for bibliography management
- Required LaTeX packages: `multirow`, `booktabs`, `natbib`, `graphicx`

### Method 1: Manual Compilation

```bash
cd /home/prototype/Downloads/Project_book

# First pass - generates .aux files
pdflatex thesis.tex

# Generate bibliography
bibtex thesis

# Second pass - includes citations and references
pdflatex thesis.tex

# Third pass - resolves all cross-references
pdflatex thesis.tex
```

### Method 2: Automatic (Recommended)

```bash
cd /home/prototype/Downloads/Project_book

# Automatically runs all necessary passes
latexmk -pdf thesis.tex
```

### Clean Build Files

```bash
# Remove auxiliary files
latexmk -c

# Remove all generated files including PDF
latexmk -C
```

---

## Diagram Export Instructions

All diagrams are created using draw.io and stored in `/tmp/Project_folder/`.

### Recommended Export Settings

**For PDF (Vector - Recommended):**
- File → Export as → PDF
- ✅ Crop
- ✅ Include page background
- ❌ Transparent background
- Quality: 100%

**For PNG (Raster - Alternative):**
- File → Export as → PNG
- Width: 2400-3200 pixels
- ✅ Transparent background
- Resolution: 300 DPI
- Border Width: 10 pixels

### Export Each Diagram

1. **Flowchart:** Export `3.2_Flowchart.drawio` → `Chap3/flowchart.pdf`
2. **Workflow:** Export `3.3_Workflow_Diagram.drawio` → `Chap3/workflow.pdf`
3. **Use Case:** Export `3.4_Use_Case_Diagram.drawio` → `Chap3/usecase.pdf`
4. **Activity:** Export `3.5_Activity_Diagram.drawio` → `Chap3/activity.pdf`
5. **Sequence:** Export `3.6_Sequence_Diagram.drawio` → `Chap3/sequence.pdf`
6. **DFD Level 0:** Export `3.7_DFD_Level_0_1_2.drawio` (Tab 1) → `Chap3/dfd_level0.pdf`
7. **DFD Level 1:** Export `3.7_DFD_Level_0_1_2.drawio` (Tab 2) → `Chap3/dfd_level1.pdf`
8. **DFD Level 2:** Export `3.7_DFD_Level_0_1_2.drawio` (Tab 3) → `Chap3/dfd_level2.pdf`
9. **ER Diagram:** Export `3.8_3.9_ER_Diagram.drawio` → `Chap3/er_diagram.pdf`

**Target Directory:** Place all exported diagrams in:
```
/home/prototype/Downloads/Project_book/Chap3/
```

---

## File Structure

```
Project_book/
├── thesis.tex                    # Main document file
├── bibfile.bib                   # Bibliography (18 references)
├── rac.sty                       # Custom style file
├── Abstract/
│   └── Abstract.tex              # Abstract section
├── Chap1/
│   └── Chapter1.tex              # Introduction (5-6 pages)
├── Chap2/
│   └── Chapter2.tex              # Background Study (9-10 pages)
├── Chap3/
│   ├── Chapter3.tex              # System Design (13-15 pages)
│   ├── flowchart.pdf/png         # Figure 3.1
│   ├── workflow.pdf/png          # Figure 3.2
│   ├── usecase.pdf/png           # Figure 3.3
│   ├── activity.pdf/png          # Figure 3.4
│   ├── sequence.pdf/png          # Figure 3.5
│   ├── dfd_level0.pdf/png        # Figure 3.6
│   ├── dfd_level1.pdf/png        # Figure 3.7
│   ├── dfd_level2.pdf/png        # Figure 3.8
│   └── er_diagram.pdf/png        # Figure 3.9
├── Chap4/
│   └── Chapter4.tex              # Implementation (Pending)
├── Chap5/
│   └── Chapter5.tex              # Results & Testing (Pending)
└── README.md                     # This file
```

---

## Key Features Implemented

### AI-Powered Proctoring
- YOLOv8n object detection (6-7 FPS on CPU)
- MediaPipe facial analysis (468 landmarks)
- Dual-camera monitoring (desktop + mobile via QR code)
- Real-time violation detection (<150ms latency)

### Exam Management
- MCQ with automated grading
- CQ with manual grading interface
- File-based submissions
- A+ to F grading scale
- Automatic banning at 5 violations

### Security & Compliance
- JWT authentication with RBAC
- HTTPS/TLS encryption
- AES-256 data encryption
- GDPR, CCPA, FERPA compliance
- Audit logging

### Performance
- 82% cost reduction vs manual proctoring
- 4.3 months ROI period
- Unlimited concurrent sessions
- CPU-optimized (no GPU required)

---

## Bibliography

The document uses **IEEE citation style** with 18 references covering:
- Online proctoring research
- Computer vision technologies (YOLOv8n, MediaPipe)
- Real-time communication (WebRTC, Socket.IO)
- Authentication standards (JWT RFC 7519)
- Privacy regulations (GDPR, CCPA, FERPA)
- Market research and feasibility studies

---

## Pending Work

- [ ] Complete Chapter 4: Implementation Details
- [ ] Complete Chapter 5: Results and Testing
- [ ] Export all 9 diagrams from draw.io to PDF/PNG
- [ ] Final compilation and proofreading
- [ ] Generate final PDF for submission

---

## Document Statistics

- **Total Chapters:** 5 (3 completed, 2 pending)
- **Total Pages:** ~30-35 pages (estimated)
- **Total Tables:** 3
- **Total Figures:** 9 diagrams
- **Total References:** 18 (IEEE format)
- **Database Tables:** 21 normalized entities (3NF)

---

## Contact Information

**Student:** Humayun Ahmed
**Email:** [Add email here]
**Registration:** 19502005005

**Supervisor:** Prof. Dr. Mohammed Shakhawat Hossain
**Institution:** Daffodil Institute of IT (DIIT)
**Address:** Dhaka - 1207, Bangladesh

---

## License

This project documentation is submitted as partial fulfillment of the requirement for the degree of B.Sc. (Hon's) in Computer Science and Engineering at National University of Bangladesh.

**© 2025 Humayun Ahmed. All Rights Reserved.**

---

## Version History

- **v1.0** (January 16, 2025) - Initial submission version
  - Chapters 1-3 completed and condensed
  - 9 diagrams created in draw.io
  - 3 tables added
  - 18 references in IEEE format
  - Bibliography updated with all citations
