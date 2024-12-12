# greenland



## Dataset Structure:
Final Directory Structure:
│   ├── cross_lingual/
│   │   ├── genetics/
│   │   │   ├── all_to_all/
│   │   │       ├── all_head_to_all_tail/
│   │   │       │   ├── test.csv
│   │   │       │   ├── train.csv
│   │   │       │   ├── valid.csv
│   │   │   ├── head_to_tail/
│   │   │   │   ├── major_to_major/
│   │   │   │   │   ├── test.csv
│   │   │   │   │   ├── train.csv
│   │   │   │   │   ├── valid.csv
│   │   │   │   ├── major_to_minor/
│   │   │   │   │   ├── test.csv
│   │   │   │   │   ├── train.csv
│   │   │   │   │   ├── valid.csv
│   │   │   │   ├── minor_to_major/
│   │   │   │   │   ├── test.csv
│   │   │   │   │   ├── train.csv
│   │   │   │   │   ├── valid.csv
│   │   │       ├── minor_to_minor/
│   │   │       │   ├── test.csv
│   │   │       │   ├── train.csv
│   │   │       │   ├── valid.csv
│   │       ├── tail_to_tail/
│   │       │   ├── major_tail_to_minor_tail/
│   │       │   │   ├── test.csv
│   │       │   │   ├── train.csv
│   │       │   │   ├── valid.csv
│   │           ├── minor_tail_to_major_tail/
│   │           │   ├── test.csv
│   │           │   ├── train.csv
│   │           │   ├── valid.csv
│   │   ├── script/
│   │   │   ├── all_to_all/
│   │   │       ├── all_head_to_all_tail/
│   │   │       │   ├── test.csv
│   │   │       │   ├── train.csv
│   │   │       │   ├── valid.csv
│   │   │   ├── head_to_tail/
│   │   │   │   ├── major_to_major/
│   │   │   │   │   ├── test.csv
│   │   │   │   │   ├── train.csv
│   │   │   │   │   ├── valid.csv
│   │   │   │   ├── major_to_minor/
│   │   │   │   │   ├── test.csv
│   │   │   │   │   ├── train.csv
│   │   │   │   │   ├── valid.csv
│   │   │   │   ├── minor_to_major/
│   │   │   │   │   ├── test.csv
│   │   │   │   │   ├── train.csv
│   │   │   │   │   ├── valid.csv
│   │   │       ├── minor_to_minor/
│   │   │       │   ├── test.csv
│   │   │       │   ├── train.csv
│   │   │       │   ├── valid.csv
│   │       ├── tail_to_tail/
│   │       │   ├── major_tail_to_minor_tail/
│   │       │   │   ├── test.csv
│   │       │   │   ├── train.csv
│   │       │   │   ├── valid.csv
│   │           ├── minor_tail_to_major_tail/
│   │           │   ├── test.csv
│   │           │   ├── train.csv
│   │           │   ├── valid.csv
│       ├── word_order/
│       │   ├── all_to_all/
│       │       ├── all_head_to_all_tail/
│       │       │   ├── test.csv
│       │       │   ├── train.csv
│       │       │   ├── valid.csv
│       │   ├── head_to_tail/
│       │   │   ├── major_to_major/
│       │   │   │   ├── test.csv
│       │   │   │   ├── train.csv
│       │   │   │   ├── valid.csv
│       │   │   ├── major_to_minor/
│       │   │   │   ├── test.csv
│       │   │   │   ├── train.csv
│       │   │   │   ├── valid.csv
│       │   │   ├── minor_to_major/
│       │   │   │   ├── test.csv
│       │   │   │   ├── train.csv
│       │   │   │   ├── valid.csv
│       │       ├── minor_to_minor/
│       │       │   ├── test.csv
│       │       │   ├── train.csv
│       │       │   ├── valid.csv
│           ├── tail_to_tail/
│           │   ├── major_tail_to_minor_tail/
│           │   │   ├── test.csv
│           │   │   ├── train.csv
│           │   │   ├── valid.csv
│               ├── minor_tail_to_major_tail/
│               │   ├── test.csv
│               │   ├── train.csv
│               │   ├── valid.csv
    ├── multilingual/
    │   ├── genetics/
    │   │   ├── all_and_all/
    │   │   │   ├── all_head_to_all_head/
    │   │   │   │   ├── test.csv
    │   │   │   │   ├── train.csv
    │   │   │   │   ├── valid.csv
    │   │   │   ├── all_tail_to_all_tail/
    │   │   │   │   ├── test.csv
    │   │   │   │   ├── train.csv
    │   │   │   │   ├── valid.csv
    │   │       ├── head_and_tail_combined/
    │   │       │   ├── test.csv
    │   │       │   ├── train.csv
    │   │       │   ├── valid.csv
    │   │   ├── head_and_head/
    │   │   │   ├── major_head_to_major_head/
    │   │   │   │   ├── test.csv
    │   │   │   │   ├── train.csv
    │   │   │   │   ├── valid.csv
    │   │       ├── minor_head_to_minor_head/
    │   │       │   ├── test.csv
    │   │       │   ├── train.csv
    │   │       │   ├── valid.csv
    │       ├── tail_and_tail/
    │       │   ├── major_tail_to_major_tail/
    │       │   │   ├── test.csv
    │       │   │   ├── train.csv
    │       │   │   ├── valid.csv
    │           ├── minor_tail_to_minor_tail/
    │           │   ├── test.csv
    │           │   ├── train.csv
    │           │   ├── valid.csv
    │   ├── script/
    │   │   ├── all_and_all/
    │   │   │   ├── all_head_to_all_head/
    │   │   │   │   ├── test.csv
    │   │   │   │   ├── train.csv
    │   │   │   │   ├── valid.csv
    │   │   │   ├── all_tail_to_all_tail/
    │   │   │   │   ├── test.csv
    │   │   │   │   ├── train.csv
    │   │   │   │   ├── valid.csv
    │   │       ├── head_and_tail_combined/
    │   │       │   ├── test.csv
    │   │       │   ├── train.csv
    │   │       │   ├── valid.csv
    │   │   ├── head_and_head/
    │   │   │   ├── major_head_to_major_head/
    │   │   │   │   ├── test.csv
    │   │   │   │   ├── train.csv
    │   │   │   │   ├── valid.csv
    │   │       ├── minor_head_to_minor_head/
    │   │       │   ├── test.csv
    │   │       │   ├── train.csv
    │   │       │   ├── valid.csv
    │       ├── tail_and_tail/
    │       │   ├── major_tail_to_major_tail/
    │       │   │   ├── test.csv
    │       │   │   ├── train.csv
    │       │   │   ├── valid.csv
    │           ├── minor_tail_to_minor_tail/
    │           │   ├── test.csv
    │           │   ├── train.csv
    │           │   ├── valid.csv
        ├── word_order/
        │   ├── all_and_all/
        │   │   ├── all_head_to_all_head/
        │   │   │   ├── test.csv
        │   │   │   ├── train.csv
        │   │   │   ├── valid.csv
        │   │   ├── all_tail_to_all_tail/
        │   │   │   ├── test.csv
        │   │   │   ├── train.csv
        │   │   │   ├── valid.csv
        │       ├── head_and_tail_combined/
        │       │   ├── test.csv
        │       │   ├── train.csv
        │       │   ├── valid.csv
        │   ├── head_and_head/
        │   │   ├── major_head_to_major_head/
        │   │   │   ├── test.csv
        │   │   │   ├── train.csv
        │   │   │   ├── valid.csv
        │       ├── minor_head_to_minor_head/
        │       │   ├── test.csv
        │       │   ├── train.csv
        │       │   ├── valid.csv
            ├── tail_and_tail/
            │   ├── major_tail_to_major_tail/
            │   │   ├── test.csv
            │   │   ├── train.csv
            │   │   ├── valid.csv
                ├── minor_tail_to_minor_tail/
                │   ├── test.csv
                │   ├── train.csv
                │   ├── valid.csv

Experiment setup completed successfully!
