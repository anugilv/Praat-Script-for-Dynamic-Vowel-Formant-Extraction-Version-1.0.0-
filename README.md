# Praat Script for Extracting Dynamic Vowel Formants (v1.0.1)

## Overview

This Praat script automates the extraction of dynamic vowel formants and other acoustic measurements from annotated speech recordings. It processes paired **WAV** and **TextGrid** files in a specified directory and extracts acoustic features based on the annotation tiers.

The script is designed for phonetic and speech science research and can be used to generate datasets for statistical analysis, visualisation, and machine learning applications.

---

## Features

The script automatically extracts:

* Dynamic formant trajectories (F1, F2, F3)
* Mean formant values (F1, F2, F3)
* Vowel duration
* Mean fundamental frequency (F0)
* Mean intensity
* Vowel labels
* Syllable labels and durations
* Word labels and durations

---

## Required File Structure

For the script to run correctly:

1. Each **WAV** file must have a corresponding **TextGrid** file with the **same filename**.

   **Example:**

   ```text
   Speaker01.wav
   Speaker01.TextGrid
   ```

2. Store the paired files in the same directory.

3. For large datasets, it is recommended to organise recordings by speaker groups (e.g., separate folders for male and female speakers), although this is optional.

---

## TextGrid Annotation Requirements

The script is designed to work with the following annotation structure:

| Tier   | Annotation |
| ------ | ---------- |
| Tier 1 | Phone      |
| Tier 2 | Syllable   |
| Tier 3 | Word       |

The script can also be adapted for TextGrids with fewer tiers by modifying the relevant tier indices in the source code.

---

## Extracted Acoustic Measurements

### Tier 1 — Phone

For each annotated vowel, the script extracts:

* Vowel label
* Vowel duration
* Dynamic F1 values (0–100% of vowel duration)
* Dynamic F2 values (0–100% of vowel duration)
* Dynamic F3 values (0–100% of vowel duration)
* Mean F1
* Mean F2
* Mean F3
* Mean fundamental frequency (F0)
* Mean intensity

---

### Tier 2 — Syllable

For the corresponding syllable:

* Syllable label
* Syllable duration

---

### Tier 3 — Word

For the corresponding word:

* Word label
* Word duration

---

## Output

The script generates a tabular output containing one row per vowel token. The output includes:

* File information
* Annotation labels
* Duration measurements
* Dynamic formant trajectories
* Mean acoustic measurements

The resulting dataset can be imported directly into software such as:

* R
* Python (Pandas)
* SPSS
* JASP
* Jamovi
* Excel

---

## Recommended Workflow

1. Prepare paired **WAV** and **TextGrid** files.
2. Verify that TextGrid annotations follow the required tier structure.
3. Open the script in Praat.
4. Specify the input directory and output filename.
5. Run the script.
6. Import the generated data into your preferred statistical software for analysis.

---

## Version

**Current Version:** **v1.0.1**

### What's New in v1.0.1

* Minor bug fixes
* Improved code stability
* Documentation updates

---

## Citation

If you use this script in your research, please cite the associated publication (if available) or acknowledge the script in your methodology section.

---

## License

This project is released under the **MIT License**.

---

## Contact

**Anugil V**

Language Analyst (Contract)

International Centre for Free and Open Source Solutions (ICFOSS), Government of Kerala, India

For questions, suggestions, or bug reports, please open an issue in this repository.

Figure 01: Ideal Tier Structure for the Script.
![Ideal Tier](https://github.com/user-attachments/assets/b03ec443-ddbd-44ae-a651-479d08960470)



   
