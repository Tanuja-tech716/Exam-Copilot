# Exam-Copilot

Exam-Copilot is a web-based application where students upload previous-year question papers (PYQs) and get a ranked list of units and topics by weightage, so they know what to study first. The first version is for 2nd-year students of VNR VJIET, Hyderabad.

**Status:** In development. Stage 1 (text extraction) is being built.

## What it will do

A student uploads a syllabus and PYQs. The app extracts the text, identifies the questions, tags each one to a topic, and shows the units and topics ranked by marks, highest first.

## Current stage: text extraction

PDFs are read page by page with PyMuPDF. Pages with too little text are treated as scanned, and images are read with Tesseract OCR. If a page cannot be read, the student is asked to upload a clearer copy. The output is a list of pages, each flagged with whether OCR was used. A blank page counts as readable.

Full design: [DESIGN.md](DESIGN.md)

## Tech Stack

- Python
- PyMuPDF
- Tesseract OCR

## Roadmap

- [ ] Stage 1: text extraction
- [ ] Stage 2: question extraction
- [ ] Stage 3: topic tagging
- [ ] Stage 4: weightage and ranked list
- [ ] Web interface
- [ ] First 5 testers