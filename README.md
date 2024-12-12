# greenland


```markdown
# GREENLAND Dataset Structure

## Cross-lingual Experiments
```
```markdown
# GREENLAND Dataset Structure

## Cross-lingual Experiments
```
cross_lingual/
├── genetics/
│   ├── head_to_tail/
│   │   ├── major_to_major/
│   │   │   ├── test.csv
│   │   │   ├── train.csv
│   │   │   └── valid.csv
│   │   ├── major_to_minor/
│   │   │   ├── test.csv
│   │   │   ├── train.csv
│   │   │   └── valid.csv
│   │   ├── minor_to_major/
│   │   │   ├── test.csv
│   │   │   ├── train.csv
│   │   │   └── valid.csv
│   │   └── minor_to_minor/
│   │       ├── test.csv
│   │       ├── train.csv
│   │       └── valid.csv
│   ├── tail_to_tail/
│   │   ├── major_tail_to_minor_tail/
│   │   │   ├── test.csv
│   │   │   ├── train.csv
│   │   │   └── valid.csv
│   │   └── minor_tail_to_major_tail/
│   │       ├── test.csv
│   │       ├── train.csv
│   │       └── valid.csv
│   └── all_to_all/
│       └── all_head_to_all_tail/
│           ├── test.csv
│           ├── train.csv
│           └── valid.csv
├── script/          # Same structure as genetics
└── word_order/      # Same structure as genetics
```

## Multilingual Experiments
```
multilingual/
├── genetics/
│   ├── head_and_head/
│   │   ├── major_head_to_major_head/
│   │   │   ├── test.csv
│   │   │   ├── train.csv
│   │   │   └── valid.csv
│   │   └── minor_head_to_minor_head/
│   │       ├── test.csv
│   │       ├── train.csv
│   │       └── valid.csv
│   ├── tail_and_tail/
│   │   ├── major_tail_to_major_tail/
│   │   │   ├── test.csv
│   │   │   ├── train.csv
│   │   │   └── valid.csv
│   │   └── minor_tail_to_minor_tail/
│   │       ├── test.csv
│   │       ├── train.csv
│   │       └── valid.csv
│   └── all_and_all/
│       ├── all_head_to_all_head/
│       │   ├── test.csv
│       │   ├── train.csv
│       │   └── valid.csv
│       ├── all_tail_to_all_tail/
│       │   ├── test.csv
│       │   ├── train.csv
│       │   └── valid.csv
│       └── head_and_tail_combined/
│           ├── test.csv
│           ├── train.csv
│           └── valid.csv
├── script/          # Same structure as genetics
└── word_order/      # Same structure as genetics
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
