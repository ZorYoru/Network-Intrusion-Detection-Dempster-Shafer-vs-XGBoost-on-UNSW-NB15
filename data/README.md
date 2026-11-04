# Data

This folder is where the **UNSW-NB15** dataset goes. The dataset is **not included** in this repository because of its size and because it belongs to its original authors.

## Files needed

Download these two files and place them directly in this folder:

| File | Records |
|---|---|
| `UNSW_NB15_training-set.csv` | 175,341 |
| `UNSW_NB15_testing-set.csv` | 82,332 |

Expected layout after download:

```
data/
├── README.md
├── UNSW_NB15_training-set.csv
└── UNSW_NB15_testing-set.csv
```

## Where to download

Official source (UNSW Canberra, Cyber Range Lab):
https://research.unsw.edu.au/projects/unsw-nb15-dataset

Use the **partitioned** training and testing sets (the two CSV files above), not the raw full capture files.

## Dataset summary

- 49 attributes per record, including the label columns `attack_cat` (attack category) and `label` (binary)
- 10 classes in `attack_cat`: Normal, Generic, Exploits, Fuzzers, DoS, Reconnaissance, Analysis, Backdoor, Shellcode, Worms
- Categorical features used in this project: `proto`, `service`, `state`

## Notes

- Both CSV files are listed in `.gitignore`, so they will not be committed by accident.
- If the notebook cannot find the files, check the path variables at the top of the notebook (`TRAIN_PATH` and `TEST_PATH`) and make sure they point to this folder.

## Citation

Moustafa, N., & Slay, J. (2015). *UNSW-NB15: a comprehensive data set for network intrusion detection systems.* Military Communications and Information Systems Conference (MilCIS).