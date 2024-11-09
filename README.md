File Conversion Application
This is a web application built using Streamlit that allows users to convert between several file formats:

PDF to Word
Word to PDF
Word to PowerPoint
PowerPoint to Word
PowerPoint to PDF
The app supports the conversion of documents and presentations between these formats, making it easy to convert files on the go.

Features
PDF to Word Conversion: Converts PDF files to Word (.docx).
Word to PDF Conversion: Converts Word files (.docx) to PDF.
Word to PowerPoint Conversion: Converts Word files (.docx) to PowerPoint presentations.
PowerPoint to Word Conversion: Converts PowerPoint presentations (.pptx) to Word documents.
PowerPoint to PDF Conversion: Converts PowerPoint presentations (.pptx) to PDF.
Requirements
Before running the app, you need to have Python 3.7 or higher installed on your system. Additionally, you will need to install the following Python libraries:

Streamlit: For building the web interface.
pdf2docx: For converting PDF to Word.
FPDF: For generating PDF files from Word documents.
python-docx: For reading and writing Word files.
python-pptx: For working with PowerPoint presentations.
Install the required libraries
You can install the required libraries using pip:

bash
Copy code
pip install streamlit pdf2docx fpdf python-docx python-pptx
Additionally, for the PowerPoint to PDF conversion, LibreOffice must be installed on your system. LibreOffice is used to convert PowerPoint files to PDFs in headless mode.

To install LibreOffice:

On Ubuntu: sudo apt-get install libreoffice
On macOS, you can install it using Homebrew: brew install --cask libreoffice
On Windows, download and install from LibreOffice.org.
How to Run the App
1. Clone the Repository (if applicable)
If you're cloning the repository, use the following command:

bash
Copy code
git clone <repository-url>
cd <repository-directory>
2. Save the Code
Save the Python code in a file named app.py in the project directory.

3. Run the Streamlit App
Once all dependencies are installed, run the following command in your terminal:

bash
Copy code
streamlit run app.py
This will start a Streamlit server, and you should see an output similar to:

arduino
Copy code
Local URL:  http://localhost:8501
Network URL:  http://<your-ip>:8501
Open the local URL (http://localhost:8501) in your browser to interact with the app.

4. Interact with the Application
Once the app is running, you can:

Choose the Conversion Type: Use the radio buttons to select one of the following conversion types:

PDF to Word
Word to PDF
Word to PowerPoint
PowerPoint to Word
PowerPoint to PDF
Upload Your File: Depending on the selected conversion type, upload the appropriate file (PDF, Word, or PowerPoint).

Download Converted File: After the conversion is complete, you'll be given the option to download the converted file (Word, PDF, or PowerPoint).

Example Usage
PDF to Word:

Upload a PDF file.
The app will convert it to a Word (.docx) file.
Download the converted Word file.
Word to PDF:

Upload a Word (.docx) file.
The app will convert it to a PDF.
Download the converted PDF file.
Word to PowerPoint:

Upload a Word (.docx) file.
The app will convert each paragraph in the Word document into a slide in a PowerPoint presentation.
Download the generated PowerPoint file.
Troubleshooting
LibreOffice Not Installed (for PowerPoint to PDF):

If you receive an error for PowerPoint to PDF conversion, make sure you have LibreOffice installed on your machine. The conversion uses LibreOffice in headless mode to generate the PDF.
Large Files Taking Too Long:

For larger files, conversions might take longer. Please be patient, as larger PDFs, Word documents, and PowerPoint presentations require more processing time.
Customizations
You can modify this app by adding more conversion types or adjusting the file handling logic.

Add More File Formats: You could add support for more file types like Excel to PDF or other common document formats.
Adjust PDF Formatting: You could enhance how the PDF is generated, adjusting fonts, margins, etc.


Acknowledgments
Streamlit: For providing the framework to build web applications.
pdf2docx: For converting PDF files to Word.
python-docx: For handling Word documents.
python-pptx: For working with PowerPoint presentations.
LibreOffice: For converting PowerPoint to PDF.
