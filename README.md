## Real-Time OCR for Hindi Text Extraction
This project focuses on developing a web-based OCR platform to extract Hindi text from scanned PDFs containing . The platform ensures that the extracted text but fails to retains the original layout, formatting, and orientation.

## Research Objectives
### Objective:
Build a web-based OCR platform capable of extracting Hindi text from scanned PDFs (e.g., voters' lists). The extracted text should be saved in the desired file format (e.g., DOCX)
### Key Focus Areas for Improvements:
- Text Extraction with Layout Preservation:
Using OCR to extract text is not sufficient for maintaining the layout, especially for documents that include tables, columns, and other complex structures. We need to enhance the OCR pipeline to keep track of the text’s location, size, and alignment.

- PDF Structure Extraction:
Before applying OCR, we should extract the layout information from the PDF. This can be achieved through tools that help retain the structure of the document, like tables and paragraphs. Using libraries like pdfminer.six or PyMuPDF, we can extract positions and coordinates of text blocks, and then later use this information to format the DOCX output.

- Text and Image Combination:
For maintaining the layout and orientation (especially for scanned documents), you can save the original images along with the extracted text, ensuring that both are available for reference when generating the final DOCX.
