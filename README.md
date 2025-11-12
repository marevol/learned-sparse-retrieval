# Learned Sparse Retrieval

A curated collection of research papers, software implementations, and resources related to learned sparse retrieval methods for information retrieval.

## Overview

This repository serves as a comprehensive reference for researchers and practitioners interested in **Learned Sparse Retrieval** - a modern approach to information retrieval that combines the efficiency of traditional sparse representations (like BM25) with the effectiveness of neural language models.

### What is Learned Sparse Retrieval?

Learned Sparse Retrieval represents a hybrid approach in information retrieval that:

- **Uses neural networks** to learn importance weights for terms in documents and queries
- **Maintains sparse representations** compatible with inverted indexes for efficient retrieval
- **Enables vocabulary expansion** through contextualized term importance estimation
- **Bridges the gap** between traditional lexical matching and dense neural retrieval

Key advantages include:
- Efficiency: Compatible with existing inverted index infrastructure
- Interpretability: Maintains explainable sparse representations
- Effectiveness: Leverages pre-trained language models for improved retrieval quality
- Scalability: Efficient first-stage retrieval for large document collections

## Table of Contents

- [Overview](#overview)
- [Papers](#papers)
  - [2019](#2019)
  - [2020](#2020)
  - [2021](#2021)
  - [2022](#2022)
  - [2023](#2023)
  - [2024](#2024)
- [Software](#software)
- [Datasets & Benchmarks](#datasets--benchmarks)
- [Related Resources](#related-resources)
- [Contributing](#contributing)

## Papers

### 2019

- Nogueira, Rodrigo, et al. "[Document expansion by query prediction.](https://arxiv.org/pdf/1904.08375)" arXiv preprint arXiv:1904.08375 (2019).
- Dai, Zhuyun, and Jamie Callan. "[Context-aware sentence/passage term importance estimation for first stage retrieval.](https://arxiv.org/pdf/1910.10687)" arXiv preprint arXiv:1910.10687 (2019).

### 2020

- Bai, Yang, et al. "[SparTerm: Learning term-based sparse representation for fast text retrieval.](https://arxiv.org/pdf/2010.00768)" arXiv preprint arXiv:2010.00768 (2020).
- Zhao, Tiancheng, Xiaopeng Lu, and Kyusong Lee. "[SPARTA: Efficient open-domain question answering via sparse transformer matching retrieval.](https://arxiv.org/pdf/2009.13013)" arXiv preprint arXiv:2009.13013 (2020).

### 2021

- Formal, Thibault, Benjamin Piwowarski, and Stéphane Clinchant. "[SPLADE: Sparse lexical and expansion model for first stage ranking.](https://arxiv.org/pdf/2107.05720)" Proceedings of the 44th International ACM SIGIR Conference on Research and Development in Information Retrieval. 2021.
- Formal, Thibault, et al. "[SPLADE v2: Sparse lexical and expansion model for information retrieval.](https://arxiv.org/pdf/2109.10086)" arXiv preprint arXiv:2109.10086 (2021).
- Lin, Jimmy, and Xueguang Ma. "[A few brief notes on deepimpact, coil, and a conceptual framework for information retrieval techniques.](https://arxiv.org/pdf/2106.14807)" arXiv preprint arXiv:2106.14807 (2021).
- Mallia, Antonio, et al. "[Learning passage impacts for inverted indexes.](https://dl.acm.org/doi/pdf/10.1145/3404835.3463030)" Proceedings of the 44th International ACM SIGIR Conference on Research and Development in Information Retrieval. 2021.

### 2022

- Formal, Thibault, et al. "[From distillation to hard negative sampling: Making sparse neural ir models more effective.](https://arxiv.org/pdf/2205.04733)" Proceedings of the 45th international ACM SIGIR conference on research and development in information retrieval. 2022.
- Lassance, Carlos, and Stéphane Clinchant. "[An efficiency study for SPLADE models.](https://arxiv.org/pdf/2207.03834)" Proceedings of the 45th International ACM SIGIR Conference on Research and Development in Information Retrieval. 2022.
- Lin, Jimmy. "[A proposed conceptual framework for a representational approach to information retrieval.](https://arxiv.org/pdf/2110.01529)" ACM SIGIR Forum. Vol. 55. No. 2. New York, NY, USA: ACM, 2022.
- Choi, Eunseong, et al. "[SpaDE: Improving sparse representations using a dual document encoder for first-stage retrieval.](https://arxiv.org/pdf/2209.05917)" Proceedings of the 31st ACM International Conference on Information & Knowledge Management. 2022.

### 2023

- Qiao, Yifan, et al. "[Optimizing Guided Traversal for Fast Learned Sparse Retrieval.](https://dl.acm.org/doi/pdf/10.1145/3543507.3583497)" Proceedings of the ACM Web Conference 2023. 2023.
- Kong, Weize, et al. "[Sparseembed: Learning sparse lexical representations with contextual embeddings for retrieval.](https://dl.acm.org/doi/pdf/10.1145/3539618.3592065)" Proceedings of the 46th International ACM SIGIR Conference on Research and Development in Information Retrieval. 2023.

### 2024

- Lassance, Carlos, et al. "[Two-Step SPLADE: Simple, Efficient and Effective Approximation of SPLADE.](https://arxiv.org/pdf/2404.13357)" European Conference on Information Retrieval. Cham: Springer Nature Switzerland, 2024.

## Software

- [SPLADE](https://github.com/naver/splade) - Official implementation of SPLADE models by Naver Labs
- [LSR: A unified framework for efficient and effective learned sparse retrieval](https://github.com/thongnt99/learned-sparse-retrieval) - Unified framework supporting multiple learned sparse retrieval methods

## Datasets & Benchmarks

Commonly used datasets and benchmarks for evaluating learned sparse retrieval methods:

### Information Retrieval Benchmarks

- **MS MARCO** - Large-scale information retrieval datasets
  - [MS MARCO Passage Ranking](https://microsoft.github.io/msmarco/) - Passage retrieval benchmark
  - [MS MARCO Document Ranking](https://microsoft.github.io/msmarco/) - Document retrieval benchmark

- **BEIR** - Heterogeneous benchmark for zero-shot evaluation
  - [BEIR: A Heterogeneous Benchmark for Information Retrieval](https://github.com/beir-cellar/beir) - Evaluation across 18 diverse datasets

- **TREC Collections** - Traditional IR test collections
  - TREC Deep Learning Track
  - TREC-COVID
  - Robust04

### Question Answering

- **Natural Questions** - Open-domain question answering dataset
- **TriviaQA** - Question answering from web snippets
- **SQuAD** - Stanford Question Answering Dataset

## Related Resources

### Tutorials & Surveys

- [Pretrained Transformers for Text Ranking: BERT and Beyond](https://arxiv.org/abs/2010.06467) - Comprehensive survey including sparse retrieval methods
- [Neural Information Retrieval: A Literature Review](https://arxiv.org/abs/1611.06792) - Overview of neural IR approaches

### Related Approaches

- **Dense Retrieval**: DPR, ANCE, ColBERT, DRAGON
- **Traditional Sparse Methods**: BM25, TF-IDF
- **Hybrid Approaches**: Combining sparse and dense retrieval

### Tools & Libraries

- [Pyserini](https://github.com/castorini/pyserini) - Python toolkit for reproducible IR research (supports sparse retrieval)
- [Anserini](https://github.com/castorini/anserini) - Lucene-based IR toolkit
- [PyTerrier](https://github.com/terrier-org/pyterrier) - Python API for Terrier IR platform

## Contributing

Contributions are welcome! If you know of relevant papers, software implementations, or resources related to learned sparse retrieval, please feel free to:

1. **Open an issue** with suggestions for new additions
2. **Submit a pull request** with your proposed changes

### Guidelines

- Papers should be peer-reviewed or from reputable preprint archives (arXiv, etc.)
- Include proper citations with links to papers when available
- Organize papers chronologically by publication year
- For software, include a brief description of what the implementation provides
- Ensure resources are directly relevant to learned sparse retrieval methods

## License

This repository is maintained as an educational and research resource. Please refer to individual papers and software repositories for their respective licenses.

## Contact

For questions or suggestions, please open an issue in this repository.
