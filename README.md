# LOOM: A Long-horizon-orientated Fusion Paradigm for Vision-Language-Action Model

[![GitHub](https://img.shields.io/badge/GitHub-Repository-blue?logo=github)](https://github.com/tonywang-0517/loom)
[![Project](https://img.shields.io/badge/Project-Page-green)](https://tonywang-0517.github.io/loom.github.io/)

Project page for **LOOM: A Long-horizon-orientated Fusion Paradigm for Vision-Language-Action Model**.

A persistent global LOOM query paradigm that maintains task intent across all policy layers for long-horizon manipulation, achieving significant improvements in success rates on long-horizon tasks and exhibiting strong generalization capabilities.

## Overview

Long-horizon, language-guided robotic manipulation requires generating coherent action sequences while effectively utilizing the semantic and compositional knowledge encoded in large vision–language models. LOOM introduces a persistent global LOOM query paradigm, in which a single global LOOM query is shared across all policy layers to aggregate and reuse vision–language constraints throughout action generation.

**Key Innovation:**
- **Persistent Global LOOM Query Paradigm**: A single global LOOM query shared across all policy layers, aggregating and maintaining vision-language constraints from all VLM layers as a stable structure throughout action generation, providing a stronger inductive bias for sustaining instruction-following behavior over extended horizons.

## Key Results

- **98.4%** average success rate on LIBERO benchmark
- **97.5%** success rate on LIBERO-Long (+1.1% improvement over VLA-Adapter-Pro)
- **82.0%** success rate on CALVIN (5 tasks in a row, +5.5% improvement over VLA-Adapter-Pro)
- **215.8 Hz** inference speed with **99.1M** parameters
- Strong generalization capabilities on long-horizon manipulation tasks

## Links

- **Project Page**: [https://tonywang-0517.github.io/loom.github.io/](https://tonywang-0517.github.io/loom.github.io/)
- **GitHub Repository**: [https://github.com/tonywang-0517/loom](https://github.com/tonywang-0517/loom)
- **Paper**: [Coming soon]
- **Video**: [Coming soon]

## Project Structure

```
loom.github.io/
├── index.html              # Main project page
├── static/
│   ├── css/               # Stylesheets
│   │   └── index.css      # Main stylesheet
│   ├── js/                # JavaScript files
│   ├── images/            # Images and visualizations
│   │   └── favicon.ico    # Site favicon
│   └── videos/            # Demo videos (if any)
└── README.md              # This file
```

## Features

- **Hero Section**: Eye-catching introduction with project title and authors
- **Abstract**: Summary of the LOOM approach and key contributions
- **Performance Highlights**: Interactive cards showcasing key success rates on LIBERO and CALVIN
- **Framework Overview**: Visual diagram of the LOOM architecture
- **Core Innovation**: Detailed explanation of Persistent Global LOOM Query Paradigm
- **Methodology**: Description of the persistent global LOOM query design and integration
- **Main Results**: Comprehensive comparison tables on LIBERO and CALVIN benchmarks
- **Ablation Studies**: Feature combination analysis, layer-wise performance, and query token number analysis

## Citation

```bibtex
@article{loom2025,
  title={LOOM: A Long-horizon-orientated Fusion Paradigm for Vision-Language-Action Model},
  author={[Authors]},
  journal={[Conference/Journal]},
  year={2025},
  url={https://tonywang-0517.github.io/loom.github.io/}
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

### Images
- Framework diagram: `../fig/framework.png` (referenced from parent directory)
- Layer-wise performance: `../fig/four_conditions.png`
- Query token analysis: `../fig/query_number.png`

## Acknowledgments

This project page design was inspired by the [ODYSSEY](https://github.com/) project page and built using the [Academic Project Page Template](https://github.com/eliahuhorwitz/Academic-project-page-template).

## Website License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
