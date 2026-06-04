# AI-Powered Book Cover Validation Workflow

## Overview

This project automates the review and validation of book cover submissions using n8n, OpenAI Vision, Airtable, Google Drive, and Gmail.

The workflow automatically analyzes uploaded covers, extracts ISBN information, validates publishing requirements, tracks revisions, and notifies authors of approval or required corrections.

---

## Features

### Automated Cover Validation

The system checks:

* Award badge overlap detection
* Author name placement validation
* Safe margin compliance
* Border spacing violations
* Text alignment issues
* Image quality and readability
* Resolution and pixelation checks

### ISBN Extraction

The workflow extracts ISBN numbers directly from uploaded cover images using OpenAI Vision.

### Intelligent Classification

Submissions are categorized as:

* PASS
* REVIEW NEEDED

### Severity Levels

Issues are classified as:

* CRITICAL
* HIGH
* MEDIUM
* LOW

### Revision Tracking

Each submission is stored in Airtable with:

* ISBN
* Submission Number
* Validation Status
* Confidence Score
* Issues Identified
* Correction Instructions

This preserves the complete review history.

---

## Tech Stack

* n8n
* OpenAI GPT-4o Vision
* Airtable
* Google Drive
* Gmail

---

## Workflow Architecture

Google Drive Upload

↓

Google Drive Trigger

↓

Download Cover File

↓

OpenAI Vision Analysis

↓

ISBN Extraction

↓

Airtable Tracking

↓

PASS / REVIEW NEEDED Classification

↓

Email Notification

---

## Future Enhancements

* Human review dashboard
* Knowledge base integration (RAG)
* Cover annotation and issue highlighting
* Analytics dashboard
* Multi-user publishing workflow

---

## Author

Praveen Kumar
