# MERAG-System(Multimodal Educational RAG System)

An AI-powered educational assistant that understands textbooks and student handwritten notes using multimodal Retrieval-Augmented Generation (RAG).

## 📌 Project Overview

Conventional text-based RAG systems mainly process digitally available text. However, educational materials also contain important information in handwritten notes, scanned pages, diagrams, tables, images, and mathematical equations.

This project develops a Multimodal Educational RAG System that can process two types of PDF documents: normal digital PDFs and handwritten PDFs. The system extracts and understands textual and visual information, retrieves relevant evidence, and generates educational responses grounded in the student's learning materials.

The system is designed to support normal PDFs containing text, tables, diagrams, images, and equations, as well as handwritten PDFs containing handwritten text, tables, diagrams, images, and equations.

## 🎯 Objectives

- Process normal digital PDFs and handwritten PDFs.
- Extract and understand text, images, diagrams, tables, and mathematical equations.
- Recognize handwritten text using models such as TrOCR.
- Store textual and visual information in a multimodal vector database.
- Retrieve relevant evidence for student questions.
- Generate educational explanations using a Large Language Model.
- Provide quiz generation and interactive learning support.
- Compare multimodal retrieval with conventional text-only RAG.

## 🚀 Key Features

### 1. Normal PDF Processing

The system accepts digital educational PDFs such as textbooks, lecture notes, and study materials.

- Extract digital text from PDF documents.
- Identify and process tables, diagrams, images, and equations.
- Preserve original pages as visual evidence.
- Generate text and image embeddings.

### 2. Handwritten PDF Processing

The system accepts PDFs containing student handwritten notes and handwritten educational content.

- Convert PDF pages into images.
- Recognize handwritten text using TrOCR.
- Process handwritten tables, diagrams, images, and equations.
- Preserve original handwritten pages as visual evidence.
- Generate text and image embeddings.

### 3. Multimodal Retrieval

- Text embeddings for textual content.
- Image embeddings for visual information.
- Vector database storage with document metadata.
- Retrieval of relevant textual and visual evidence.
- Reranking of retrieved evidence before response generation.

### 4. AI Educational Tutor

- Question answering from textbooks and handwritten notes.
- Context-grounded educational explanations.
- Quiz generation.
- Interactive learning through a single AI tutor.

## 🔄 System Workflow

```text
Student Uploads PDF
        |
        v
PDF Type and Page Analysis
        |
        v
   ┌───────────────┬────────────────┐
   |               |                |
Normal PDF    Handwritten PDF       |
   |               |                |
Digital Text   Page Image           |
Extraction     Conversion           |
   |               |                |
   |          Handwriting           |
   |          Recognition           |
   |               |                |
   └───────────────┴────────────────┘
                   |
                   v
       Tables / Diagrams / Images /
             Equations
                   |
                   v
       Multimodal Embedding
              Generation
                   |
                   v
        Multimodal Vector Database
                   |
                   v
           Student Question
                   |
                   v
          Evidence Retrieval
                   |
                   v
              Reranking
                   |
                   v
           Large Language Model
                   |
                   v
         Educational Response
```

## 🏗️ System Architecture

### Document Processing Layer

- PDF type and page analysis.
- Digital text extraction.
- Handwritten text recognition.
- Tables, diagrams, images, and equation processing.

### Multimodal Representation Layer

- Text embedding generation.
- Image embedding generation.
- Document metadata creation.

### Retrieval Layer

- Multimodal vector indexing.
- Relevant evidence retrieval.
- Evidence reranking.

### Generation Layer

- Large Language Model.
- Grounded educational responses.

### Educational Application Layer

- Student interaction.
- Question answering.
- Quiz generation.

## 🛠️ Technologies

| Component | Technology |
|---|---|
| Programming Language | Python |
| PDF Processing | PDF parsing and image extraction tools |
| Handwritten Text Recognition | TrOCR |
| Text Embeddings | Text embedding model |
| Image Embeddings | Image embedding model |
| Vector Database | Qdrant |
| Retrieval-Augmented Generation | RAG |
| Language Model | LLM |
| Frontend | React |
| Backend | FastAPI |


## 📚 Research Foundation

This project is based on research in multimodal retrieval-augmented generation and educational document understanding.

### Base Paper

**RAG-Anything: All-in-One RAG Framework**

Authors: Z. Guo, X. Ren, L. Xu, J. Zhang, and C. Huang.
link: https://arxiv.org/abs/2510.12323

### Other References

