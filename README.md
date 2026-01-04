# MIRAGE: Masked Imitation for Robotic Action Generation and Execution

[![GitHub](https://img.shields.io/badge/GitHub-Repository-blue?logo=github)](https://github.com/tonywang-0517/Mirage)
[![Project](https://img.shields.io/badge/Project-Page-green)](https://tonywang-0517.github.io/mirage.github.io/)

Project page for **MIRAGE: Masked Imitation for Robotic Action Generation and Execution** by Puyue Wang (University of Auckland, ICML 2026).

A lightweight execution framework for robust whole-body humanoid control with standardized data, achieving substantially higher success rates under domain shifts and enabling reliable zero-shot sim-to-sim transfer to unseen physics engines.

## Overview

Achieving robust whole-body humanoid control under dynamics mismatch remains a central challenge in robotics. MIRAGE introduces two key innovations:

- **SCHEMA** (Sparse Command Handling for Embodied Motion Abstraction): A standardized sparse-joint protocol based on SMPL-X keypoints that consolidates fragmented motion sources into a single training and execution format
- **MIRROR** (Memory-Integrated Robust Representation for Online Robustness): A history-conditioned control policy that leverages recent state–action sequences as implicit dynamics memory, significantly improving stability and sim-to-sim transfer

## Key Results

- **90.7%** success rate in training simulator (IsaacLab)
- **86.0%** success rate in zero-shot transfer to unseen physics engine (Genesis)
- Significantly outperforms strong baselines including MaskedMimic, OmniH2O, ExBody2, and Hover
- Robust performance across six representative motions under zero-shot domain transfer

## Links

- **Project Page**: [https://tonywang-0517.github.io/mirage.github.io/](https://tonywang-0517.github.io/mirage.github.io/)
- **GitHub Repository**: [https://github.com/tonywang-0517/Mirage](https://github.com/tonywang-0517/Mirage)
- **Paper**: [Overleaf](https://www.overleaf.com/read/ttjqpnkhmyrv#3c1420)
- **Video**: [YouTube](https://www.youtube.com/watch?v=YOUR_VIDEO_ID) (Coming soon)
- **Author**: [Puyue Wang](https://github.com/tonywang-0517)

## Project Structure

```
mirage.github.io/
├── index.html              # Main project page
├── static/
│   ├── css/               # Stylesheets
│   │   └── index.css      # Main stylesheet with sand/gold theme variables
│   ├── js/                # JavaScript files
│   ├── images/            # Images and visualizations
│   │   ├── bg.png                      # Hero section background
│   │   ├── mirage_overview.png         # Framework overview
│   │   ├── teacher_training_stage1.jpg # Training stage 1
│   │   ├── student_training_stage2.jpg # Training stage 2
│   │   ├── mirage_eval_process.jpg     # Evaluation process
│   │   ├── method_comparison.png       # Ablation training curves
│   │   ├── metrics_comparison1.png     # Training metrics comparison
│   │   ├── all_metrics_eval_combined.png # Ablation results on Genesis
│   │   ├── terrain.png                 # Terrain diversity
│   │   └── favicon.ico                 # Site favicon
│   └── videos/            # Demo videos
│       ├── eval/           # Evaluation videos
│       │   ├── 1_punch/mirage/tmp_video.mp4
│       │   ├── 2_getup/mirage/tmp_video.mp4
│       │   ├── 3_high_kick/mirage/tmp_video.mp4
│       │   ├── 4_common_walk/mirage/tmp_video.mp4
│       │   ├── 5_side_walk/mirage/tmp_video.mp4
│       │   └── 6_martial/mirage/tmp_video.mp4
│       ├── g1_random_push.mp4          # Random perturbation recovery
│       ├── masked_mimic_g1_no_vae.mp4  # Teacher-student distillation
│       └── ...
└── README.md              # This file
```

## Features

- **Hero Section**: Eye-catching introduction with custom background image
- **Performance Highlights**: Interactive cards showcasing key success rates
- **Two Core Innovations**: Detailed explanation of SCHEMA and MIRROR
- **Training Methodology**: Two-stage teacher-student training architecture with domain randomization
- **Sim-to-Sim Transfer Performance**: Comprehensive comparison table with baselines
- **Ablation Studies**: Component analysis, training curves, and test results
- **Representative Motion Demonstrations**: Six motion videos under zero-shot domain transfer
- **Policy Structure Comparison**: Method comparison table
- **Live Demonstrations**: Robust recovery and expert distillation videos
- **Evaluation Framework**: Comprehensive testing visualization
- **Terrain Diversity**: Analysis across varied environmental conditions

## Citation

```bibtex
@inproceedings{wang2026mirage,
  title={MIRAGE: Masked Imitation for Robotic Action Generation and Execution},
  author={Wang, Puyue},
  booktitle={Proceedings of the 39th International Conference on Machine Learning (ICML)},
  year={2026},
  organization={University of Auckland},
  url={https://github.com/tonywang-0517/Mirage}
}
```

## Development

The project page uses modern web technologies:
- **Bulma CSS** framework for responsive design
- **Font Awesome** for icons
- **Bulma Carousel** for image/video carousels
- **Custom CSS variables** for sand/gold theme consistency
- **CSS gradient styles** for visual appeal
- Optimized for performance and SEO

### Theme Colors

The page uses a sand/gold color theme defined in CSS variables:
- Primary color: `#e8c99b` (light sand gold)
- Primary hover: `#d4a574` (medium sand gold)
- Primary dark: `#b8864a` (dark sand gold)
- All colors are centrally managed through CSS variables in `static/css/index.css`

## Media Assets

### Images
All images are properly referenced and positioned:
- `bg.png` - Hero section background image
- `mirage_overview.png` - Framework overview diagram
- `teacher_training_stage1.jpg` - Stage 1 training visualization
- `student_training_stage2.jpg` - Stage 2 training visualization
- `mirage_eval_process.jpg` - Evaluation methodology visualization
- `method_comparison.png` - Ablation training curves comparison
- `metrics_comparison1.png` - Training metrics comparison
- `all_metrics_eval_combined.png` - Ablation results on Genesis test dataset
- `terrain.png` - Terrain diversity analysis

### Videos
- **Evaluation Videos**: Six representative motions (punch, get up, high kick, common walk, side walk, martial) under zero-shot domain transfer
- `g1_random_push.mp4` - Random perturbation recovery demonstration
- `masked_mimic_g1_no_vae.mp4` - Teacher-student distillation demonstration

## Acknowledgments

This project page design was inspired by the [ODYSSEY](https://github.com/) project page and built using the [Academic Project Page Template](https://github.com/eliahuhorwitz/Academic-project-page-template).

## Website License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
