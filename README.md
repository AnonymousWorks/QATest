# QATest

QATest is a tool using novel sentence-level mutation based metamorphic testing, which can precisely detect bugs in
QA software.


## Reproducibility


### Environment build
0. download datasets 
1. build SLAHAN environment following the tutorial [SLAHAN](https://github.com/kamigaito/SLAHAN)
2. install all python dependent packages for QATest
```
pip install -r requirements.txt
```


### Run QATest

0. run SLAHAN to compress the seed question into a short question. 
The compressed questions are saved in path `datasets/compress`

1. run QATest to generate all new test cases and detect bugs. 
The results are saved in path `QATest/results/`

```
cd ../script/
python run.py project_name  # valid project_name are 'boolq', 'squad2', 'narrative' 
```




