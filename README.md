Instructions for Using the Praat Script for Extracting Dynamic Vowel Formants (Version 1.0.0)

This Praat script automates the extraction of various acoustic parameters from annotated speech data. It processes TextGrid and WAV files from a specified directory, extracting formant values and other acoustic features based on different annotation tiers.

I. Required File Setup:

1. Ensure each WAV file has a corresponding TextGrid file in the same directory.
   
2. It is recommended that the files be organized by speaker gender (e.g., separate folders for male and female speakers).
   
3. The annotation structure should ideally contain three tiers: Phone (Tier 1), Syllable (Tier 2), and Word (Tier 3). However, the script can function with fewer tiers by altering the script.
   
II. Extracted Features by Annotation Tiers:

1. Phone Tier (Tier 1):
   
   a. Dynamic vowel formant values (F1, F2, F3) extracted at multiple time points (0%–100% of vowel duration).
   
   b. Vowel duration and label.
   
   c. Mean values of F1, F2, and F3 across the vowel duration.
   
   d. Mean fundamental frequency (F0).
   
   e. Mean intensity (I).

3. Syllable and Word Tiers (Tiers 2 and 3):
   
   a. Duration and label of the corresponding syllable.
   
   b. Duration and label of the corresponding word.

Figure 01: Ideal Tier Structure for the Script.
![Ideal Tier](https://github.com/user-attachments/assets/b03ec443-ddbd-44ae-a651-479d08960470)



   
