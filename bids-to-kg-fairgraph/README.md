Scripts to automatically create and upload OpenMINDS schemes to Knowledge Graph based on dataset in BIDS structure

```
bidsdir
├── code
├── sourcedata
│   ├── dataset.dvc
│   └── dataset
│       └── sub-01
│           ├── ses-01
│           │   └── t1wc
│           │       └── *.dcm
│           └── ses-02
│               └── t1wc
│                   └── *.dcm
├── rawdata
│   ├── dataset.dvc
│   └── dataset
│       └── sub-01
│           ├── ses-01
│           │   └── t1wc.nii.gz
│           └── ses-02
│               └── t1wc.nii.gz
└── derivatives
    ├── dataset-mni.dvc
    └── dataset-mni
        └── sub-01
            ├── ses-01
            │   └── t1wc.nii.gz
            └── ses-02
                └── t1wc.nii.gz
```
# Add metadata to existing DatasetVersion scheme
Edit update-graph.py and tokens in environment.txt, then run with
```
bash update-graph.sh
```
