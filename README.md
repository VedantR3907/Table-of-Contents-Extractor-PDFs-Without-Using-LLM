![TOC Extractor](app/utils/images_and_videos/toc_banner.png)

# Table of Contents Extractor from PDFs Without Using LLM

## Overview

The **TOC Extractor** is a Python-based tool that extracts the Table of Contents (TOC) from PDF files without relying on machine learning (ML), deep learning (DL), or large language models (LLMs).

It uses logical Python code, text-processing rules, and regex patterns to identify and extract TOC content from PDFs.

For a detailed explanation of how the tool works, refer to the [blog post](https://medium.com/@vedantrajpurohit3907/the-toc-extractor-from-pdfs-b42a3df8236a).

---

## Demo Video

[Watch the demo video](https://youtu.be/5uJsEpJkgdY)

---

## Installation Guide

### Branches Overview

This repository has two branches for different use cases:

- **`main` branch**: Contains the core code along with sample PDFs for testing, covering domains such as IT, Finance, and Storybooks.
- **`TOC_Extactor_without_testing_PDFs` branch**: Contains only the core code without sample PDFs, intended for testing with custom PDFs.

> **Note**: The branch name `TOC_Extactor_without_testing_PDFs` contains the spelling `Extactor`. Use the branch name exactly as it exists in GitHub when cloning.

---

### Clone the Repository

Use one of the following commands depending on your requirement.

#### Main Branch — With Sample PDFs

```bash
git clone https://github.com/VedantR3907/Table-of-Contents-Extractor-PDFs-Without-Using-LLM.git
```

#### `TOC_Extactor_without_testing_PDFs` Branch — Without Sample PDFs

```bash
git clone --branch TOC_Extactor_without_testing_PDFs https://github.com/VedantR3907/Table-of-Contents-Extractor-PDFs-Without-Using-LLM.git
```

---

### Install Dependencies

After cloning the repository, navigate to the project directory:

```bash
cd Table-of-Contents-Extractor-PDFs-Without-Using-LLM
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

---

## Usage

### 1. Prepare PDF Files

Place your PDF files inside the `Data` folder located in the main directory of the project.

```text
Table-of-Contents-Extractor-PDFs-Without-Using-LLM/
├── Data/
│   ├── sample_1.pdf
│   ├── sample_2.pdf
│   └── ...
```

---

### 2. Run the Script

Navigate to the `app` folder:

```bash
cd app
```

Run the main script:

```bash
python main.py
```

---

### 3. View the Output

After execution, the extracted results will be saved in the `output` folder.

The output folder follows this structure:

```text
output/
├── 01/                     # Output from the first filter
├── 02/                     # Output from the second filter
├── Filters_03/             # Outputs from sub-filters in the third stage
│   ├── 01/
│   ├── 02/
│   ├── 03/
├── extracted_content/      # Extracted content from the PDFs
└── Final_output/           # Final TOC text files for each PDF
```

The `Final_output` folder contains the final extracted Table of Contents text files for all processed PDFs.

> **Note**: Refer to the [blog post](https://medium.com/@vedantrajpurohit3907/the-toc-extractor-from-pdfs-b42a3df8236a) for a detailed explanation of the extraction stages and filters.

---

## Maintenance

### Cleaning Output Folders

To clear all generated output files, navigate to the `utils` folder:

```bash
cd utils
```

Run the cleanup script:

```bash
python clear_output_folders.py
```

---

## Project Structure

```text
Table-of-Contents-Extractor-PDFs-Without-Using-LLM/
├── app/
│   ├── main.py
│   ├── utils/
│   │   ├── images_and_videos/
│   │   │   └── toc_banner.png
│   │   └── clear_output_folders.py
│   └── ...
├── Data/
│   └── PDF files
├── output/
│   ├── 01/
│   ├── 02/
│   ├── Filters_03/
│   ├── extracted_content/
│   └── Final_output/
├── requirements.txt
└── README.md
```

---

## Features

- Extracts Table of Contents from PDF files
- Does not use ML, DL, or LLM-based techniques
- Uses logical Python code and regex-based filtering
- Supports multiple PDFs
- Provides staged output for better debugging and understanding
- Includes a cleanup utility for generated outputs
- Suitable for testing on PDFs from multiple domains

---

## Additional Information

- Make sure your Python environment is correctly set up before running the project.
- Install all required dependencies using `requirements.txt`.
- Place input PDF files inside the `Data` folder before running the script.
- Final extracted TOC files will be available inside the `output/Final_output` folder.
- For issues, suggestions, or contributions, use the GitHub repository.

---

## Repository

GitHub Repository: [Table-of-Contents-Extractor-PDFs-Without-Using-LLM](https://github.com/VedantR3907/Table-of-Contents-Extractor-PDFs-Without-Using-LLM)
