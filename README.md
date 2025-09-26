# README for the SYNTH Initiative

_Ultimate Synthetic Multilingual Open Data Corpus for Frontier Sovereign AI Models and Agentic Applications_

> [Published Documentation](https://the-ai-alliance.github.io/SYNTH-initiative/)

The SYNTH initiative aims to address the critical gap in open-source AI development by creating a cutting-edge, open-source data corpus for training sovereign AI models and advanced AI agents. This involves curating permissively licensed, high-quality multilingual datasets, with a focus on underrepresented languages, and generating synthetic data specifically designed to enhance frontier-level reasoning capabilities in these languages. The ultimate mission is to enable global access to advanced AI reasoning by fostering an inclusive data ecosystem that supports the full training pipeline of sophisticated AI systems, thereby reducing dependency on proprietary data and closed models.

## Problem to address

Current open source AI development faces a fundamental asymmetry. Large-scale pretraining datasets like The Pile, FineWeb or Dolma have enabled the creation of capable base models. However, the transition from base models to frontier-grade systems and exceptional agentic applications requires specialized datasets for:

- Midtraining: Domain-specific, multi-modal, high-quality data that bridges general pretraining and task-specific fine-tuning, crucial for advancing downstream models and context relevant AI agents  
- Reinforcement Learning: Training data for developing advanced reasoning capabilities, including multi-step problem solving, mathematical reasoning, and complex analytical tasks, increasingly useful in agentic workflows  
- Frontier Reasoning Development: High-quality examples of sophisticated reasoning chains, logical inference patterns, and systematic problem decomposition 


These critical training phases currently rely heavily on proprietary datasets or synthetic data generated from closed frontier models, creating a dependency that undermines the open-source ecosystem's ability to develop advanced reasoning capabilities independently.

## Goals

1. **Curate Permissively Licensed Seed Collections**

The SYNTH initiative identifies and aggregates *exceptional quality, multilingual, domain specific* *datasets with permissive licensing* that ensures unrestricted sharing, auditing, and future use. This includes expanding upon foundational resources like Pleias's Common Corpus while specifically targeting underrepresented languages from Eastern Europe, Asia, Africa, and other regions. The focus is on building reasoning capabilities across diverse linguistic contexts, as current frontier reasoning models exhibit significant performance gaps in lower-resource languages, limiting their global applicability for complex problem-solving tasks.

2. **Generate Synthetic Data for Multilingual Frontier Reasoning Models**

SYNTH provides a platform to develop systematic approaches to create high-quality synthetic datasets for midtraining and reinforcement learning that specifically target advanced reasoning capabilities across multiple languages, particularly lower-resource ones. This is crucial because reasoning capabilities‚Äîmathematical problem-solving, logical inference, multi-step analytical thinking‚Äîare often severely degraded or entirely absent in underrepresented languages. The generation process must leverage diverse, high-quality multilingual open seed data rather than relying solely on closed frontier models, ensuring the resulting synthetic corpus maintains openness while achieving the quality and linguistic diversity necessary for training models capable of sophisticated reasoning across all languages.

3. **Enable Sovereign AI and Agentic Applications Development**

The SYNTH initiative creates the data infrastructure necessary for regions and organizations to develop culturally and linguistically aligned, technologically advanced AI models and agents with strong reasoning capabilities in their native languages. This addresses the critical gap where current frontier reasoning models perform well primarily in English and a few high-resource languages, leaving billions of speakers unable to access sophisticated AI reasoning in their native languages.

## Expected Impact

SYNTH initiative will provide the missing link in open AI development: the specialized, high-quality datasets necessary to transform capable base models into frontier-grade reasoning systems. By ensuring permissive licensing throughout the pipeline, we preserve the ability for global researchers, organizations, and regions to build, audit, and customize AI systems that serve their specific needs and values.

The result will be a comprehensive data ecosystem that supports not just model pretraining, but the full spectrum of advanced training techniques necessary for developing AI systems with sophisticated reasoning capabilities that are both technically advanced and globally inclusive.


## Getting Involved

We welcome contributions as PRs. Please see our [Alliance community repo](https://github.com/The-AI-Alliance/community/) for general information about contributing to any of our projects. This section provides some specific details you need to know.

In particular, see the AI Alliance [CONTRIBUTING](https://github.com/The-AI-Alliance/community/blob/main/CONTRIBUTING.md) instructions. You will need to agree with the AI Alliance [Code of Conduct](https://github.com/The-AI-Alliance/community/blob/main/CODE_OF_CONDUCT.md).

All _code_ contributions are licensed under the [Apache 2.0 LICENSE](https://github.com/The-AI-Alliance/community/blob/main/LICENSE.Apache-2.0) (which is also in this repo, [LICENSE.Apache-2.0](LICENSE.Apache-2.0)).

All _documentation_ contributions are licensed under the [Creative Commons Attribution 4.0 International](https://github.com/The-AI-Alliance/community/blob/main/LICENSE.CC-BY-4.0) (which is also in this repo, [LICENSE.CC-BY-4.0](LICENSE.CC-BY-4.0)).

All _data_ contributions are licensed under the [Community Data License Agreement - Permissive - Version 2.0](https://github.com/The-AI-Alliance/community/blob/main/LICENSE.CDLA-2.0) (which is also in this repo, [LICENSE.CDLA-2.0](LICENSE.CDLA-2.0)).

### Quick Tip - View the Website Locally

See [GITHUB_PAGES.md](GITHUB_PAGES.md) for information on viewing the site locally with `jekyll`.

### We use the "Developer Certificate of Origin" (DCO).

> [!WARNING]
> Before you make any git commits with changes, understand what's required for DCO.

See the Alliance contributing guide [section on DCO](https://github.com/The-AI-Alliance/community/blob/main/CONTRIBUTING.md#developer-certificate-of-origin) for details. In practical terms, supporting this requirement means you must use the `-s` flag with your `git commit` commands.

## About the GitHub Pages Website Published from this Repo

The website is published using [GitHub Pages](https://pages.github.com/), where the pages are written in Markdown and served using [Jekyll](https://github.com/jekyll/jekyll). We use the [Just the Docs](https://just-the-docs.github.io/just-the-docs/) Jekyll theme.

See [GITHUB_PAGES.md](GITHUB_PAGES.md) for more information.

> [!NOTE]
> As described above, all documentation is licensed under Creative Commons Attribution 4.0 International. See [LICENSE.CDLA-2.0](LICENSE.CDLA-2.0)).
