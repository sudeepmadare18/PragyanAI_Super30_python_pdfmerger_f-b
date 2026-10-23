# PDF Merger Web Application Using Frontend And Backend

A web-based application that allows users to upload multiple PDF files and merge them into a single PDF document. The frontend is developed using HTML, CSS, and JavaScript, while the backend is developed using Python FastAPI and pypdf.

## Problem Statement

Users often have multiple PDF files related to the same document, such as assignments, reports, certificates, invoices, or study materials. Managing and sharing these files separately can be difficult. Many offline PDF merger tools require installation, and some online tools are not user-friendly. Therefore, there is a need for a simple web-based application that allows users to merge multiple PDF files quickly and easily.

## Project Description

This project allows users to upload two or more PDF files and merge them into one PDF document. The frontend collects the selected PDF files and sends them to the FastAPI backend. The backend uses the pypdf library to merge all uploaded PDF files into a single PDF. After merging, the user can download the final merged PDF file.

The frontend is developed using HTML, CSS, and JavaScript. The backend is developed using Python FastAPI. The application is deployed using Netlify.

## Features

- Upload multiple PDF files
- Merge PDF files into one document
- Download the final merged PDF
- Simple and user-friendly web interface
- Fast processing using FastAPI
- Frontend and backend separation
- Deployed using Netlify

## Technologies Used

- HTML
- CSS
- JavaScript
- Python
- FastAPI
- Uvicorn
- pypdf
- python-multipart
- Netlify

## Project Structure

```text
PDF-Merger-Project/
│
├── backend/
│   ├── main.py
│   ├── utils.py
│   ├── config.json
│   └── requirements.txt
│
└── frontend/
    ├── index.html
    ├── script.js
    └── style.css
```

- `main.py` — Contains FastAPI routes and API logic  
- `utils.py` — Contains PDF merging functions  
- `config.json` — Stores configuration details  
- `requirements.txt` — Contains required Python libraries  
- `index.html` — Creates the frontend page structure  
- `style.css` — Styles the web page  
- `script.js` — Handles file upload and backend communication  

## Backend Requirements

```text
fastapi
uvicorn[standard]
pypdf
python-multipart
```

- **FastAPI** — Used to create the backend API  
- **Uvicorn** — Used to run the FastAPI server  
- **pypdf** — Used to merge PDF files  
- **python-multipart** — Used to handle file uploads  

## Workflow

1. User opens the PDF Merger web application.
2. User selects two or more PDF files.
3. JavaScript sends the selected files to the FastAPI backend.
4. Backend receives the uploaded PDF files.
5. pypdf merges all PDF files in order.
6. A single merged PDF file is generated.
7. Merged PDF is sent back to the frontend.
8. User downloads the final merged PDF.

## How to Run

1. Clone this repository:
   ```bash
   git clone <your-repository-link>
   ```

2. Install backend requirements:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the FastAPI backend:
   ```bash
   uvicorn main:app --reload
   ```

4. Open the frontend `index.html` file in a browser or deploy it using Netlify.

## Output

- User can upload multiple PDF files.
- The application merges all selected PDF files.
- A single merged PDF file is generated.
- User can download the final merged PDF.

## Live Application

[https://projectpdfmerger.netlify.app/]

## Future Scope

- Add option to rearrange PDF files before merging
- Add PDF split feature
- Add PDF compression feature
- Add password protection for merged PDF
- Add preview of PDF pages
- Add drag-and-drop file upload option

## Developed By

[Sudeep S]
