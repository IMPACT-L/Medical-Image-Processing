# Final Project Guidelines

This document provides a practical workflow for ELEC 444 / ELEC 6661 final projects. Official instructor announcements and Moodle take precedence.

## 1. Goal

Use medical-imaging data to solve or investigate a concrete problem using methods covered in the course or closely related techniques.

Good projects are **focused, reproducible and measurable**. A smaller experiment with a strong baseline and careful analysis is usually more useful than a very large project that cannot be reproduced.

## 2. Suggested project types

### Paper reproduction + extension

- Select a published medical-imaging paper.
- Reproduce an important baseline/result.
- Add one meaningful extension, comparison or ablation.
- Explain what changed and why.

### Classical medical-image processing

Examples include:

- denoising
- edge detection
- segmentation
- registration
- similarity metrics
- RANSAC-based estimation
- clustering

### Machine/deep learning project

Examples include:

- classification
- detection
- segmentation
- registration
- representation learning
- explainability
- transformer/ViT-based analysis

## 3. Minimum reproducibility checklist

Your repository should make it possible for another student to understand how the reported results were produced.

Include:

- problem statement
- dataset name and access instructions
- preprocessing description
- baseline/model description
- environment/dependencies
- training or inference command
- evaluation command
- metrics
- representative qualitative results
- references

Do **not** commit patient-identifiable data, private clinical data, credentials, API keys or large datasets to GitHub.

## 4. Recommended experiment structure

A strong experiment usually contains:

1. **Baseline** — a known method or simple reference system.
2. **Your contribution/analysis** — improvement, new comparison, changed component, or targeted study.
3. **Evaluation** — appropriate quantitative metrics.
4. **Qualitative examples** — useful images/overlays when appropriate.
5. **Ablation or controlled comparison** — isolate the effect of important design choices.
6. **Limitations** — explain failure cases and constraints.

## 5. Metrics by task

Choose metrics appropriate to your task. Examples:

- **Segmentation:** Dice, IoU/Jaccard, sensitivity, specificity, Hausdorff distance
- **Classification:** accuracy, balanced accuracy, precision, recall, F1, AUROC
- **Registration:** target registration error, landmark error, Dice after alignment, similarity metric
- **Denoising/reconstruction:** PSNR, SSIM, task-specific quality measures

Do not choose metrics only because they make the result look better. Explain why they fit the medical-imaging task.

## 6. Suggested repository layout

```text
project-name/
├── README.md
├── requirements.txt
├── configs/
├── data/              # preferably ignored; include instructions, not private data
├── notebooks/
├── src/
│   ├── data/
│   ├── models/
│   ├── train.py
│   └── evaluate.py
├── results/
│   ├── figures/
│   └── tables/
└── docs/              # GitHub Pages/project report assets
```

## 7. Final project page/report

A clear project page should answer:

- What medical problem are you solving?
- What dataset did you use?
- What baseline did you start from?
- What did you change or investigate?
- How was it evaluated?
- What are the main quantitative results?
- What do qualitative examples show?
- What are the limitations?
- How can the work be reproduced?

See [GitHub Pages Guide](GITHUB_PAGES_GUIDE.md) and the included project template.

## 8. Undergraduate / graduate scope

The official course page notes that ELEC 444 undergraduate students may implement a paper or choose a RANSAC-based project. ELEC 6661 graduate projects should be substantially more demanding.

Project scope should be discussed with the instructor/POD when uncertain.

## 9. Important dates

- **Final project due:** December 1, 2026, 11:59 PM
- **Student presentations:** December 3, 2026
