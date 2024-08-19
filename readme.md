# RS-Coreset

## Requirement
python3+  
pytorch  
numpy  
sklearn  
matplotlib  

## Usage

### For Yield Prediction

#### For your own dataset
1. Prepare an xlsx file of reaction data in SMILES format according to the given style.
2. Convert the reaction space into a binary npy file (we provide a basic molecular fingerprint conversion script in utils).
3. Modify the arguments in `class Arguments` of `main.py`
4. run `main.py` and the prediction result will be represent as `result.csv`

#### For our real world dataset

Download and unzip `reaction93.zip` in current dir from https://drive.google.com/file/d/1O_Qcn5Z2gwr5e93Uh694d7d5HK3spkJo/view?usp=drive_link
```
python yield_predict_real.py
```

### For performance test
We prepare BH.py, SM.py and BH_Plus.py for performance test on these three public HTE dataset  
Download and unzip `datasets.zip` in current dir from [https://drive.google.com/drive/folders/1Dioh_fcPyMbhNNtEmNyUE4TrzxMnXgkV?usp=sharing](https://drive.google.com/file/d/1LGjips42xvGdOU_8pzS3quciIiXiYLfz/view?usp=drive_link)  
```
python BH.py
python SM.py
python BH_Plus.py
```
