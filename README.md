# AI-Powered Question Generator for E-Learning System

This project is an AI-powered application that extracts text from uploaded files (PDF, TXT, DOCX) and generates multiple-choice questions (MCQs) using Google's Generative AI models. The generated MCQs are presented in the web interface and can be downloaded as text or PDF files.

---

## Features
- Upload files in PDF, TXT, or DOCX formats.
- Extract and preprocess the text content.
- Generate MCQs with a question and four answer options (one correct and three distractors).
- Download generated MCQs as a `.txt` or `.pdf` file.

---

## Prerequisites
Ensure the following are installed on your system:
- Python 3.7+
- Flask
- `pdfplumber`
- `python-docx`
- `fpdf`
- `google-generativeai`

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/lakruwan1/AI-Powered-Question-Generator-App.git
   cd AI-Powered-Question-Generator-App
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate # For Linux/Mac
   venv\Scripts\activate   # For Windows
   ```

3. Install required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up Google Generative AI API key:
   - Replace `YOUR_GOOGLE_API_KEY` in the code with your actual API key.

---

## Project Structure
- **app.py**: Main application file containing the Flask web app logic.
- **templates/index.html**: Front-end template for the upload and input form.
- **templates/results.html**: Front-end template for displaying generated MCQs and download options.
- **uploads/**: Directory for storing uploaded files.
- **results/**: Directory for storing generated MCQ files.

---

## Usage

1. Run the application:
   ```bash
   python app.py
   ```

2. Open your browser and go to:
   ```
   http://127.0.0.1:5000
   ```

3. Steps to generate MCQs:
   - Upload a file (PDF, TXT, or DOCX).
   - Specify the number of questions to generate.
   - Click on the "Generate" button.

4. Review the generated MCQs and download the results in `.txt` or `.pdf` format.

---

## Sample Workflow
1. **Upload File**: Provide a document containing the text content for MCQ generation.
2. **Process File**: Text is extracted and analyzed to identify question-worthy content.
3. **Generate MCQs**: Using Google's AI models, MCQs are created with clear questions and options.
4. **Download Results**: MCQs are saved as `.txt` or `.pdf` for easy access.

---

## Technologies Used
- **Backend**: Flask
- **Text Extraction**: `pdfplumber`, `python-docx`
- **MCQ Generation**: Google Generative AI (Gemini Model)
- **File Handling**: `fpdf`, Python file handling modules
- **Frontend**: HTML, CSS (Flask templates)

---

## Known Issues and Limitations
- The AI model relies on the text quality extracted from the document; noisy or poorly scanned documents may lead to suboptimal results.
- API quota limits may apply depending on your Google Generative AI account.

---

## Future Improvements
- Add support for more file formats.
- Improve question generation by customizing prompt engineering.
- Implement user authentication and history management for generated results.

---

## Contributing
Contributions are welcome! Feel free to open issues or submit pull requests to improve this project.

---

## License
This project is licensed under the [MIT License](LICENSE).

---

## Contact
For any inquiries or support, please contact:
- **Name**: Lakruwan Kasun
- **Email**: lakruwankasun0407@gmail.com
