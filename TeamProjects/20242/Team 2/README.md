(project repository: https://github.com/ccss17/analysis_gender_text)

# Dataset

- [dataset](https://drive.google.com/file/d/12tzd1j9a7-kUSGOsMgZn15JbU-dMEq_x/view?usp=sharing): text dataset extracted from images
- [output](https://drive.google.com/file/d/1nFLe8H_SITwSgUujDENt2dSWNqvBv7Ja/view?usp=sharing): preprocessed dataset
- [result](https://drive.google.com/file/d/1VEBeAsPnRqJ0XZyGWo53sHwxpH6O9ZEX/view?usp=sharing): result csv files

# Installation

## 01_DataPreparation.py

- install tesseract(https://github.com/tesseract-ocr/tesseract#installing-tesseract)
- install python packages(`PIL`, `pytesseract`, `requests`, `bs4`)

## 02_DataPreprocessing.R

- install mecab-ko(https://r2bit.com/bitNLP/articles/Install_mecab.html)

- install [`ccss17/bitNLP`](https://github.com/ccss17/bitNLP)

    ```R
    install.packages("remotes")
    remove.packages("bitNLP")
    remotes::install_github("ccss17/bitNLP")
    install_mecab_ko()
    install.packages("RcppMeCab")
    ```

- install necessary R library

    ```R
    install.packages("magrittr")
    install.packages("dplyr")
    install.packages("parallel")
    install.packages("stringr")
    install.packages("tm")
    ```

## 03_DataAnalysis.R

- install necessary R library

    ```R
    install.pakcages("magrittr")
    install.pakcages("dplyr")
    install.pakcages("tm")
    install.pakcages("str2str")
    install.pakcages("tidyr")
    install.pakcages("slam")
    install.pakcages("wordcloud2")
    ```

# Result

## Setting 1(window size: 7, rank weight step: 0.02)

- male

    ![](img/(7,0.02)male.png)

- female

    ![](img/(7,0.02)female.png)

- male distinguished

    ![](img/(7,0.02)male_d.png)

- female distinguished

    ![](img/(7,0.02)female_d.png)

## Setting 2(window size: 10, rank weight step: 0.1)

- male

    ![](img/(10,0.1)male.png)

- female

    ![](img/(10,0.1)female.png)

- male distinguished

    ![](img/(10,0.1)male_d.png)

- female distinguished

    ![](img/(10,0.1)female_d.png)

## Setting 3(window size: 15, rank weight step: 0.2)

- male

    ![](img/(15,0.2)male.png)

- female

    ![](img/(15,0.2)female.png)

- male distinguished

    ![](img/(15,0.2)male_d.png)

- female distinguished

    ![](img/(15,0.2)female_d.png)
