# Speaker_Recognition_EEC_201_Project

Team Job Hunters: Nathan Lai and Anthony Tan-Andia

## Executing the program
1) Download "Speech Recognition Project.ipynb" from the Github respository.
2) Upload the file to a Google Drive and open it in Google Colab
3) Click Runtime>Disconnect and delete runtime>Yes
4) Click Runtime>Run all to run the program

## Abstract
The goal of this project is to create a signal processing model that successfully
identifies speakers using the mel-frequency cepstrum coefficients and vector
quantization. The model is trained on various human voices. These voices are then
treated as signals that are processed framed using a hamming window. The STFT of
each frame is calculated, and we apply mel-frequency wrapping. From this, we are
able to caculate the mel-frequency cepstrum coefficients (mfcc) for each frame.
These coefficients are then treated as vectors that can be quantized to recognize
patterns. We apply the LGB algorithm to create centroids from various clusters
in the vector space. These centroids create a collection of codewords in a codebook
which we can use to identify the speaker. To test our model we initially used 11
audio files of different people saying the word "zero". In training we achieved
an accuracy of 100% and in testing we achieved an accuracy of 75%. We then went
on to test other features, such as the model's robustness to missing frequencies,
how it handled more speakers, and how it handled more words. 

## Human Benchmark
In our human benchmark we achieved an accuracy of 37.5%. The speaker's that we 
got correct in our initial training set were speakers 2, 3, and 5. Our accuracy
is pretty low as we had trouble remembering what each person sounded like. Some
people sounded very similar to each other while others sounded vastly different.
As a human, picking up these vocal differences during the first pass is difficult.

## Speech Processing

## Vector Quantization

## Test Results
### **Test 7**
#### **Non speaker recordings of "zero"**
Training Data Accuracy: 100%
Testing Data Accuracy: 75%

#### **Non speaker with teammates' recordings of "zero"**
Training Data Accuracy: 100%
Testing Data Accuracy: 70%

### **Test 8**
#### **Notch filter blocking 60 Hz applied to Test 7**
Testing Data Accuracy: 75%

#### **Notch filter blocking 200 Hz applied to Test 7**
Testing Data Accuracy: 62.5%

#### **Notch filter blocking 400 Hz applied to Test 7**
Testing Data Accuracy: 75%

### **Test 9**
#### **Original Speakers + 10 random Students with speech "zero"**
Training Data Accuracy: 100%
Testing Data Accuracy: 72.22%

### **Test 10a: Zero/Twelve system**
#### **Train and test with zero**
Training Data Accuracy: 100%
Testing Data Accuracy: 72.22%

#### **Train and test with twelve**
Training Data Accuracy: 100%
Testing Data Accuracy: 66.67%

#### **Train and test with zero/twelve**
Training Data Accuracy: 100%
Testing Data Accuracy: 69.44%

### **Test 10b: Five/Eleven system**
#### **Train and test with five**
Training Data Accuracy: 100%
Testing Data Accuracy: 91.3%

#### **Train and test with eleven**
Training Data Accuracy: 100%
Testing Data Accuracy: 86.96%

#### **Train and test with five/eleven**
Training Data Accuracy: 100%
Testing Data Accuracy: 89.13%
