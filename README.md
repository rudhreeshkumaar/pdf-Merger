# PDF Merger

This Python script uses the `PyPDF2` library to merge multiple PDF files into a single PDF document. It combines all the PDF files present in the current working directory and creates a new file named "combined.pdf" that contains the merged content.

## Prerequisites

Make sure you have the `PyPDF2` library installed. You can install it using `pip`:

```
pip install PyPDF2
```

## Usage

1. Save the script in a Python file, e.g., `pdf_merger.py`.
2. Place all the PDF files you want to merge in the same directory as the script.
3. Execute the script in your preferred Python environment.

## Script Description

1. The script imports the `PyPDF2` library, which is used for PDF manipulation.
2. It creates a `PdfFileMerger` object called `merger`, which will be used to merge the PDF files.
3. The script then iterates through all the files in the current working directory using `os.listdir(os.curdir)`.
4. For each file with a `.pdf` extension, it appends the file to the `merger` object using `merger.append(file)`.
5. After appending all the PDF files, the script writes the merged content to a new file named "combined.pdf" using `merger.write("combined.pdf")`.

## Note

- Make sure to place only the PDF files you want to merge in the same directory as the script. Other file types may cause errors during the merging process.
- If you want to merge PDF files from a specific folder, modify the script to use the desired folder path instead of the current working directory.
- If you need to handle large PDF files or a large number of files, consider implementing additional error handling and validation to ensure smooth execution.

Enjoy using this simple PDF merger script to combine multiple PDF files into one!
