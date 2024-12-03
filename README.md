# SAL_Project
By Pranit Khanna (2021101057) and Monica Surtani (2023802005)  
The slides are already shared so not covering the project here.  
Training and test data for native dataset.  

Run the MFA_LJSpeech.ipynb file  
-> MFA installation will be done.  
-> Lbirispeech dataset will be downloaded  
-> After performing MFA on ljs dataset folder, we obtain ljs_aligned folder which has the phoneme alignments along with time stamps for all audio clips.  
-> Save the zip form of ljs_aligned folder.  
Download the ljs_aligned.zip and unzip it.  
Run the output_phonemes.ipynb  
-> NOTE: Give complete file paths.  
-> We obtain output_phonemes folder which has the phonemes with start and end time in each file for all audio clips.  
->  We obtain row_phoneme folder which has the words and phonemes with stress labels in each file for all audio clips.  
->  We obtain phoneme_sequences folder which has the words and phonemes with no stress labels in each file for all audio clips.  
->  We obtain phoneme_sequences_only folder which has the phonemes with no words in each file for all audio clips. This is used as P2TK toolkit input dataset.  
Unzip the p2tk-code-r18-python-syllabify.zip  
Copy and paste syllable_generation_folders.ipynb in the folder p2tk-code-r18-python-syllabify.  
Run syllable_generation_folders.ipynb by giving input folder phoneme_sequences_only and obtain syllables in syllable folder for all audio clips.  
Take output_phonemes folder and syllables folder as input folders for output.ipynb file and obtain required prepared data for feature extraction, training and testing purposes.  

Testing on non native dataset (ISLE DATASET)  
Download the dataset from given link  
https://iiitaphyd-my.sharepoint.com/personal/jhansi_mallela_research_iiit_ac_in/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fjhansi%5Fmallela%5Fresearch%5Fiiit%5Fac%5Fin%2FDocuments%2FResearch%2Fdata%2FhtkCorrectedLab%2Ezip&parent=%2Fpersonal%2Fjhansi%5Fmallela%5Fresearch%5Fiiit%5Fac%5Fin%2FDocuments%2FResearch%2Fdata  
Run isle.ipynb file by giving appropriate file paths according to the code requirement.( which can be understood by giving addresses in code)  
Obtain SYLLBLESTRESS AND syllablestress3 files for test data set.  

The syllables for non-native dataset is present is SYLLABLESTRESS2  
X_test and X_train consist of testing and training features respectively. (I do not remember which test this is since it was very convenient for me to switch between native and non-native test sets while running the code but I can provide both later if required.) Along with Y_test and Y_train consisting of their respective gold stress markings.  
data.pkl is the training syllables that were used.  
features.ipynb consists of extracting features and some analysis presented in the slides.  
model_training.ipynb was for training models ( stress level 2 for mfa was converted to 1 so make sure to run those cells) along with some report generation.  
Please make a note that some graphs and results may vary from the slides but that is because some experiments were being conducted by me but the results shown in the slides are only valid.  
