# Resume Reader v1

## Overview

An AI-powered resume parsing and evaluation workflow. It receives a PDF resume via webhook, extracts text using pdf.co, then branches into parallel paths: resume section extraction, job matching evaluation, and LaTeX code generation. An AI agent evaluates the resume quality, and results are merged and returned via webhook response. This provides a comprehensive resume analysis with structured section breakdown and quality scoring.

## How It Works

```
Webhook (PDF resume) -> pdf.co extract text -> Branch into: Resume Sections extraction, Job evaluation (AI Agent), LaTeX generation -> Merge results -> Respond
```

## Integrations

- **pdf.co** - PDF text extraction
- **OpenAI** - Resume evaluation and LaTeX generation

## Setup

1. Import `Resume_Reader_v1.json` into your n8n instance.
2. Configure OpenAI credentials and pdf.co API keys.
3. Activate and send POST requests with PDF resumes.
