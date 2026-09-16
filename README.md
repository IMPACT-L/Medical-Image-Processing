# Medical Image Processing — ELEC 444 / ELEC 6661 

Student-facing repository for **Medical Image Processing** at **Concordia University**.

> **Official course page:** https://users.encs.concordia.ca/~hrivaz/courses/Med_Imag_444_2026/
>
> The official course page and Moodle remain the authoritative sources. If anything here differs from an instructor announcement, follow the instructor/Moodle version.

## Course at a glance

- **Course:** ELEC 444 / ELEC 6661 — Medical Image Processing
- **Department:** Electrical and Computer Engineering, Concordia University
- **Instructor:** Prof. Hassan Rivaz
- **Time:** Thursdays, 2:45–5:15 PM
- **Undergraduate:** ELEC 444, 3 credits
- **Graduate:** ELEC 6661, 4 credits
- **PODs:** Yasaman and Omid — see Moodle for POD timing/contact information

### What the course covers

The course introduces principles and algorithms for processing and analyzing medical images, including:

- X-ray, CT, MRI, ultrasound and nuclear imaging
- Image representation and manipulation
- Convolution and aliasing
- Denoising and edge detection
- Machine learning for medical imaging
- Segmentation, RANSAC and k-means
- Medical image registration and similarity metrics
- Deep learning, explainable AI, RNN/LSTM
- Transformers and Vision Transformers in medical imaging

## Assessment

| Component | ELEC 444 | ELEC 6661 |
|---|---:|---:|
| Assignments | 10% | 10% |
| Project | 20% | 40% |
| Midterm | 20% | 20% |
| Final exam | 50% | 30% |

There are **three MATLAB assignments** and **one final project**. The final project can be implemented in a language appropriate to the project.

## Important project dates

- **Project due:** December 1, 2026 at 11:59 PM
- **Student presentations:** December 3, 2026 (Week 12)
- All undergraduate and graduate students must be present for the final class/project presentations.

See [Project Guidelines](docs/PROJECT_GUIDELINES.md) for the recommended workflow and repository structure.

## Assignments

| Assignment | Posted | Due | Points |
|---|---|---|---:|
| 1. Matrix and image manipulation | Sep. 10, 5 PM | Sep. 23, 11:59 PM | 1.0 |
| 2. Detecting edges of brain MRI | Oct. 8, 5 PM | Oct. 19, 11:59 PM | 4.5 |
| 3. Segmentation of brain MRI | Nov. 5, 5 PM | Nov. 18, 11:59 PM | 4.5 |

## Weekly schedule

| Week / Date | Topic |
|---|---|
| Week 1 — Sep. 10 | Logistics; introduction to X-ray, CT and nuclear imaging |
| Week 2 — Sep. 17 | Ultrasound and MR imaging; images in MATLAB |
| Week 3 — Sep. 24 | Convolution; aliasing in medical images |
| Week 4 — Oct. 1 | Ultrasound imaging and contrast agents; surgical robotics |
| Week 5 — Oct. 8 | Denoising; edge detection |
| Oct. 15 | Reading week |
| Oct. 22 | Machine learning in medical imaging |
| Week 7 — Oct. 29 | **Midterm in class** |
| Week 8 — Nov. 5 | Segmentation; RANSAC; k-means |
| Week 9 — Nov. 12 | Registration; SSD, NCC, correlation ratio, joint entropy, mutual information |
| Week 10 — Nov. 19 | From linear filters to deep learning; explainable AI; RNN; LSTM |
| Week 11 — Nov. 26 | Transformers, ViT, breast lesion segmentation, AI in ultrasound |
| Week 12 — Dec. 3 | **Student presentations** |

## Final project

The project is an opportunity to apply course concepts to a real medical-imaging problem.

### Undergraduate students — ELEC 444

The official course page states that undergraduate students may:

1. implement a research paper, or
2. complete a project based on RANSAC algorithms.

Students choosing the RANSAC option should follow the specific submission/report requirements stated by the instructor.

### Graduate students — ELEC 6661

Graduate students are expected to complete a **significantly more demanding project**, consistent with the additional course credit and project weight.

### Recommended project workflow

1. Pick a clearly defined medical-imaging problem.
2. Select a public dataset or a dataset approved by the instructor.
3. Identify a reproducible baseline.
4. Reproduce the baseline before adding your own idea.
5. Introduce a meaningful extension, comparison, ablation or improvement.
6. Evaluate with suitable quantitative metrics and qualitative examples.
7. Keep the code reproducible and document dependencies and commands.
8. Prepare a clear final presentation and project page/report according to course instructions.

A starter project structure is included in [`project-template/`](project-template/).

## Medical imaging datasets

The official course page contains an extensive dataset list covering MRI, CT, ultrasound, chest X-ray, mammography, OCT/OCTA and endoscopy.

Start here:

- [Dataset guide](resources/DATASETS.md)
- [Official complete dataset list](https://users.encs.concordia.ca/~hrivaz/courses/Med_Imag_444_2026/)

## Repository map

```text
medical-image-processing-2026/
├── README.md
├── docs/
│   ├── PROJECT_GUIDELINES.md
│   └── GITHUB_PAGES_GUIDE.md
├── project-template/
│   ├── README.md
│   ├── requirements.txt
│   ├── src/
│   ├── notebooks/
│   ├── results/
│   └── docs/
├── resources/
│   ├── DATASETS.md
│   └── USEFUL_TOOLS.md
└── .gitignore
```

## Textbooks

**Textbook**  
Wolfgang Birkfellner, *Medical Image Processing*, CRC Press, 2014.

**Reference book**  
Geoff Dougherty, *Medical Image Processing*, Cambridge University Press, 2009.

## Questions

For course policy, deadlines, grading and official submission instructions, use the official course page and Moodle. For project implementation questions, use the POD support information provided on Moodle.
