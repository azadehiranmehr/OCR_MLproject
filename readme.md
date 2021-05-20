OCR Reciept project


upload receipt picture as `formdata` with `file` keyword

will receive parsed result as json response

# USAGE


## Step 1. install tesseract

### Installing tesseract on Ubuntu

```sudo apt-get update
sudo apt-get install libleptonica-dev 
sudo apt-get install tesseract-ocr
sudo apt-get install libtesseract-dev
```
[Traindata for Tesseract](https://tesseract-ocr.github.io/tessdoc/Data-Files.html)


### Installing tesseract on Windows
this version of tesserac for windows: Tesseract-ocr-w64-setup-v4.1.0.20190314.exe from:<br>
[https://digi.bib.uni-mannheim.de/tesseract/]

To install Tesseract 4  on Windows use this informative article on MEDIUM:<br>
[Installing and using Tesseract 4 on windows 10](https://medium.com/quantrium-tech/installing-and-using-tesseract-4-on-windows-10-4f7930313f82)


### Step 2. ```cd OCR_Receipt```
   
### Step 3. ```pipenv install```

### Step 4. ```pipenv shell```

### Step 5. ```./src/manage.py migrate```

### Step 6. ```./src/manage.py runserver```

### step 7.install postman to send post request

### Step 8. at postman `endpoint`: "127.0.0.1:8000/api/predictor/"  , KEY=`file`  ,  VALUE = select file to upload receipt picture