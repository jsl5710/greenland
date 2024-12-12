# greenland

```markdown
# GREENLAND Dataset Structure\n
\n
## Dataset Organization\n
\n
| Experiment Type | Category | Split Type | Subset | Files |
|----------------|----------|------------|---------|-------|
| Cross-lingual | Genetics/Script/Word Order | head_to_tail | major_to_major | train.csv, valid.csv, test.csv |
| | | | major_to_minor | train.csv, valid.csv, test.csv |
| | | | minor_to_major | train.csv, valid.csv, test.csv |
| | | | minor_to_minor | train.csv, valid.csv, test.csv |
| | | tail_to_tail | major_tail_to_minor_tail | train.csv, valid.csv, test.csv |
| | | | minor_tail_to_major_tail | train.csv, valid.csv, test.csv |
| | | all_to_all | all_head_to_all_tail | train.csv, valid.csv, test.csv |
| Multilingual | Genetics/Script/Word Order | head_and_head | major_head_to_major_head | train.csv, valid.csv, test.csv |
| | | | minor_head_to_minor_head | train.csv, valid.csv, test.csv |
| | | tail_and_tail | major_tail_to_major_tail | train.csv, valid.csv, test.csv |
| | | | minor_tail_to_minor_tail | train.csv, valid.csv, test.csv |
| | | all_and_all | all_head_to_all_head | train.csv, valid.csv, test.csv |
| | | | all_tail_to_all_tail | train.csv, valid.csv, test.csv |
| | | | head_and_tail_combined | train.csv, valid.csv, test.csv |
\n
## Directory Structure\n
\n
### Cross-lingual Experiments\n
```
cross_lingual/\n
├── genetics/\n
│   ├── head_to_tail/\n
│   │   ├── major_to_major/\n
│   │   │   ├── test.csv\n
│   │   │   ├── train.csv\n
│   │   │   └── valid.csv\n
│   │   ├── major_to_minor/\n
│   │   │   ├── test.csv\n
│   │   │   ├── train.csv\n
│   │   │   └── valid.csv\n
│   │   ├── minor_to_major/\n
│   │   │   ├── test.csv\n
│   │   │   ├── train.csv\n
│   │   │   └── valid.csv\n
│   │   └── minor_to_minor/\n
│   │       ├── test.csv\n
│   │       ├── train.csv\n
│   │       └── valid.csv\n
│   ├── tail_to_tail/\n
│   │   ├── major_tail_to_minor_tail/\n
│   │   │   ├── test.csv\n
│   │   │   ├── train.csv\n
│   │   │   └── valid.csv\n
│   │   └── minor_tail_to_major_tail/\n
│   │       ├── test.csv\n
│   │       ├── train.csv\n
│   │       └── valid.csv\n
│   └── all_to_all/\n
│       └── all_head_to_all_tail/\n
│           ├── test.csv\n
│           ├── train.csv\n
│           └── valid.csv\n
├── script/          # Same structure as genetics\n
└── word_order/      # Same structure as genetics\n
```\n
\n
### Multilingual Experiments\n
```
multilingual/\n
├── genetics/\n
│   ├── head_and_head/\n
│   │   ├── major_head_to_major_head/\n
│   │   │   ├── test.csv\n
│   │   │   ├── train.csv\n
│   │   │   └── valid.csv\n
│   │   └── minor_head_to_minor_head/\n
│   │       ├── test.csv\n
│   │       ├── train.csv\n
│   │       └── valid.csv\n
│   ├── tail_and_tail/\n
│   │   ├── major_tail_to_major_tail/\n
│   │   │   ├── test.csv\n
│   │   │   ├── train.csv\n
│   │   │   └── valid.csv\n
│   │   └── minor_tail_to_minor_tail/\n
│   │       ├── test.csv\n
│   │       ├── train.csv\n
│   │       └── valid.csv\n
│   └── all_and_all/\n
│       ├── all_head_to_all_head/\n
│       │   ├── test.csv\n
│       │   ├── train.csv\n
│       │   └── valid.csv\n
│       ├── all_tail_to_all_tail/\n
│       │   ├── test.csv\n
│       │   ├── train.csv\n
│       │   └── valid.csv\n
│       └── head_and_tail_combined/\n
│           ├── test.csv\n
│           ├── train.csv\n
│           └── valid.csv\n
├── script/          # Same structure as genetics\n
└── word_order/      # Same structure as genetics\n
```\n
\n
## Data Split Details\n
\n
| Split Type | Description |
|------------|-------------|
| train.csv | Training dataset (80% for multilingual, 90% for cross-lingual) |
| valid.csv | Validation dataset (10%) |
| test.csv | Test dataset (10% for multilingual, 100% of target languages for cross-lingual) |
\n
## Category Descriptions\n
\n
| Category | Description |
|----------|-------------|
| Genetics | Language family-based splits |
| Script | Writing system-based splits |
| Word Order | Syntactic structure-based splits |
```

Each category (genetics, script, word_order) follows identical internal structure but with different language splits based on their respective criteria:

1. **Genetic Splits**: Based on language families
2. **Script Splits**: Based on writing systems
3. **Word Order Splits**: Based on syntactic structure

Every terminal directory contains:
- `train.csv`: Training dataset
- `valid.csv`: Validation dataset
- `test.csv`: Test dataset
```

## File Structure Notes

Each experiment type (cross-lingual and multilingual) contains three main categories:
1. **Genetics**: Language family-based splits
2. **Script**: Writing system-based splits
3. **Word Order**: Syntactic structure-based splits

### Cross-lingual Splits
- **head_to_tail/**: Testing transfer from high-resource to low-resource languages
- **tail_to_tail/**: Testing transfer between low-resource languages
- **all_to_all/**: Comprehensive cross-resource evaluation

### Multilingual Splits
- **head_and_head/**: Transfer between high-resource languages
- **tail_and_tail/**: Transfer between low-resource languages
- **all_and_all/**: Combined resource level transfers

### Data Files
Each split contains three files:
- `train.csv`: Training data
- `valid.csv`: Validation data
- `test.csv`: Test data
```
