# GitHub Pages Project Guide

A project page is a compact way to communicate your final work and link the results to reproducible code.

## Recommended sections

1. **Title and team**
2. **Problem statement**
3. **Motivation / clinical context**
4. **Dataset**
5. **Method**
6. **Experimental setup**
7. **Results**
8. **Qualitative examples**
9. **Discussion and limitations**
10. **Reproducibility**
11. **References**

## Simple setup

For a standard GitHub repository:

1. Put the project page in `docs/index.md`.
2. On GitHub, open **Settings → Pages**.
3. Under **Build and deployment**, select **Deploy from a branch**.
4. Select the main branch and `/docs` folder.
5. Save the setting.

GitHub will provide the project-page URL after deployment.

## Figures

Keep final figures in `docs/assets/` and use descriptive filenames.

Example:

```markdown
![Segmentation examples](assets/segmentation_examples.png)
```

Every figure should have a useful caption and enough context to understand what is being shown.

## Results table example

```markdown
| Method | Dice ↑ | HD95 ↓ |
|---|---:|---:|
| Baseline | 0.81 | 8.4 |
| Proposed experiment | 0.85 | 6.9 |
```

Replace example values with your actual results.

## Reproducibility section

Include short commands such as:

```bash
pip install -r requirements.txt
python src/train.py --config configs/baseline.yaml
python src/evaluate.py --checkpoint checkpoints/best.pt
```

Do not publish private datasets, patient-identifying information, passwords, tokens or credentials.
