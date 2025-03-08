# Speaker_Recognition_EEC_201_Project
## Executing the program
1) Download "Speech Recognition Project.ipynb" from the Github respository.
2) Upload the file to a Google Drive and open it in Google Colab
3) Click Runtime>Disconnect and delete runtime>Yes if it is available
4) Click Runtime>Run all to run the program

## Accuracy Results
### **Test 7**
#### **Non speaker recordings of "zero"**
Training Data Accuracy: 100%
Testing Data Accuracy: 75%

#### **Non speaker with teammates' recordings of "zero"**
Training Data Accuracy: 100%
Testing Data Accuracy: 77.77%

### **Test 8**
#### **Notch filter blocking 60 Hz applied to Test 7**
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
