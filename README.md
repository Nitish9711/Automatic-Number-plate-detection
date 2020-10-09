# Automatic Number plate detection

---

## Table of Contents
- [About](#about)
- [Installation Prerequisites](#installation-prerequisites)
- [How to Run this Website](#how-to-run-this-website)


---
## About
This program detects and extract the Vehicle Number using TESSERACT OCR ENGINE. Image undergoes different operations to extract the image.
1. First it take image as input.
    ![Sample image](/sample.jpg)
    <br>

2. Converts the image into grayscale. 
    ![Grey scale](/gray.png)
    <br>
3. Contour mapping. 
    ![Contour mapping](/contour_mapping.png)
    <br>

3. Conversion to black and white image according to threshold value.
    ![black and white](/black_white.png)
    <br> 

4. Inverting image and final output
    ![Inverted Image](/output.png)
    <br>

5. Text Extraction 
    - Output is then passed to Tesseract which will detect all the text in the image
    - filteration of all the text we got to vehicle number



---
## Installation Prerequisites
- python
>To Download python  [Go to the python Download Website](https://www.python.org/downloads/).

- Tesseract 

> To install Tesseract 32 bit version click on the [link](https://digi.bib.uni-mannheim.de/tesseract/tesseract-ocr-w32-setup-v5.0.0-alpha.20200328.exe)

> To install Tesseract 64 bit version click on the [link](https://digi.bib.uni-mannheim.de/tesseract/tesseract-ocr-w64-setup-v5.0.0-alpha.20200328.exe)

---

## How to Run 
1. Clone this Repo to your Local Machine.
2. Open The Terminal/CMD in the clonned folder.
3. type ```py -m pip install -r requirements.txt'``` to install all the required libraries.
4. For detecting vehicle number in the sample image.
    a. type ```python OCR.py sample.jpg``` in the Terminal/CMD.
5. For detecting vehicle number in image.    
    a. Paste the image you want to detect vehicle number in the current directory.
    b. Type ```python OCR.py [image_name]```.
6. Vehicle number printed in Terminal/CMD.
