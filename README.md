# Praat Script for Extracting Dynamic Vowel Formants (v1.0.1)

A Praat script for automatically extracting dynamic vowel formants and other acoustic measurements from annotated speech recordings.

---

## Overview

This script automates the extraction of acoustic features from paired **WAV** and **TextGrid** files. It is designed for phonetic and speech science research, enabling efficient extraction of vowel formants, durations, pitch, intensity, and annotation information for downstream statistical analysis.

The script processes an entire directory of recordings and generates a tabular output that can be imported into **R**, **Python**, **Excel**, **SPSS**, **JASP**, or **Jamovi**.

---

## Features

The script extracts:

* Dynamic F1, F2, and F3 trajectories
* Mean F1, F2, and F3
* Mean fundamental frequency (F0)
* Mean intensity
* Vowel duration
* Phone labels
* Syllable labels and durations
* Word labels and durations

---

# File Preparation

Before running the script, ensure the following requirements are met.

## 1. File Pairing

Each **WAV** file must have a corresponding **TextGrid** file with the **same filename**.

**Example**

```text
Speaker01.wav
Speaker01.TextGrid
```

Both files should be stored in the same directory.

---

## 2. Folder Organisation

For large corpora, it is recommended to organise recordings by speaker groups (e.g., separate folders for male and female speakers). This is optional but simplifies corpus management.

---

## 3. TextGrid Structure

The script is designed to work with the following three-tier annotation structure.

| Tier   | Annotation |
| ------ | ---------- |
| Tier 1 | Phone      |
| Tier 2 | Syllable   |
| Tier 3 | Word       |

### Ideal Tier Structure

![Ideal Tier Structure](https://github.com/user-attachments/assets/b03ec443-ddbd-44ae-a651-479d08960470)

**Figure 1.** Ideal TextGrid tier structure required by the script.

> **Note**
>
> The script assumes the tier order shown above. If your TextGrid uses a different tier order or contains fewer tiers, you will need to modify the tier indices in the Praat script accordingly.

---

# Acoustic Measurements

## Tier 1 – Phone

For every vowel interval, the script extracts:

* Phone label
* Vowel duration
* Dynamic F1 (0–100% of vowel duration)
* Dynamic F2 (0–100% of vowel duration)
* Dynamic F3 (0–100% of vowel duration)
* Mean F1
* Mean F2
* Mean F3
* Mean F0
* Mean intensity

---

## Tier 2 – Syllable

For the corresponding syllable:

* Syllable label
* Syllable duration

---

## Tier 3 – Word

For the corresponding word:

* Word label
* Word duration

---

# Output

The script generates a tab-delimited output file where each row represents a vowel token and includes:

* File information
* Annotation labels
* Duration measurements
* Dynamic formant trajectories
* Mean acoustic measurements

The output can be imported directly into statistical software for further analysis.

---

# Recommended Workflow

1. Prepare paired **WAV** and **TextGrid** files.
2. Verify the TextGrid tier structure.
3. Open the script in Praat.
4. Specify the input folder and output filename.
5. Run the script.
6. Analyse the extracted data in your preferred statistical software.

---

# Version

**Current Release:** **v1.0.1**

### Changes in v1.0.1

* Minor bug fixes
* Improved stability
* Updated documentation

---

# Citation

If you use this script in academic work, please cite the associated publication (if available) or acknowledge this repository in your methodology section.

---

# License

This project is distributed under the **MIT License**.

---

# Author

**Anugil V**

Language Analyst (Contract)

International Centre for Free and Open Source Solutions (ICFOSS), Government of Kerala, India
