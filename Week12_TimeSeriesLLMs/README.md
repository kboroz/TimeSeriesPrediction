# LLMs for Time Series

ALL REQUIRED:

https://www.youtube.com/watch?v=tH3Vig7YYwg

https://www.youtube.com/watch?v=_gFycwbfS0g

https://www.youtube.com/watch?v=Mf2FOzDPxck

https://www.youtube.com/watch?v=265Mpaj8O1U

https://www.youtube.com/watch?v=Zyj8iFSK7xY

https://www.youtube.com/watch?v=jyrOmIiI2Bc

OPTIONAL:

https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi

xLSTMTime:

The xLSTMTime Paper

A primary paper focusing on this architecture is "xLSTMTime: Long-Term Time Series Forecasting with xLSTM" (Afrasiabi et al., 2024). This research adapts the Extended Long Short-Term Memory (xLSTM) framework specifically for long-term time series forecasting (LTSF).

    Key Innovation: The paper introduces xLSTMTime, which leverages the exponential gating and revised matrix memory structure (mLSTM) of the original xLSTM to handle the temporal dependencies of time series data more effectively than traditional LSTMs.

    Performance: It demonstrates that refined recurrent architectures can offer competitive, and sometimes superior, alternatives to Transformer-based models in LTSF tasks by providing a linear memory footprint and faster inference (Afrasiabi et al., 2024).

LOTSA:

The LOTSA Dataset and MOIRAI

The LOTSA dataset is the cornerstone of the paper "Unified Training of Universal Time Series Forecasting Transformers" (Woo et al., 2024), which introduced the MOIRAI model.

    Dataset Scale: LOTSA is one of the largest open-source time series archives, containing over 27 billion observations across nine diverse domains (Woo et al., 2024).

    Connection to xLSTM: While the original MOIRAI paper focused on a Transformer-based architecture, the emergence of the LOTSA dataset has provided a new "gold standard" for testing large-scale time series models like xLSTM. Recent benchmarks and follow-up studies in early 2026 have begun evaluating xLSTM-based architectures against MOIRAI using the LOTSA archive to test their "zero-shot" and "any-variate" forecasting capabilities.

References

    Afrasiabi, S., Nasiri, M., & Mousavi, B. (2024). xLSTMTime: Long-term time series forecasting with xLSTM. AI, 5(3), 1482–1495.

    Woo, G., Liu, C., Sahoo, D., Kumar, A., & Hoi, S. (2024). Unified training of universal time series forecasting transformers. arXiv preprint arXiv:2402.02592.

    Beck, M., Pöppel, K., & Hochreiter, S. (2024). xLSTM: Extended long short-term memory. arXiv preprint arXiv:2405.04517.

Since its release in mid-2024, the LOTSA (Large-scale Open Time Series Archive) dataset—containing 27 billion observations—has become the standard benchmark for training and evaluating Time Series Foundation Models (TSFMs) (Woo et al., 2024).

The following five papers represent the most recent (2025–2026) research utilizing or benchmarking against the LOTSA archive:
1. "It’s TIME: Towards the Next Generation of Time Series Forecasting Benchmarks"

    Published: February 2026

    Significance: This paper introduces a new, rigorous benchmarking framework to address "data leakage" in older datasets (Brigato et al., 2026). It evaluates the performance of several models trained on LOTSA, including TiRex, an xLSTM-based model, against newer foundation models like Chronos-2 and TimesFM 2.5 (Brigato et al., 2026).

    Key Model Tested: TiRex (xLSTM architecture).

2. "Moirai-2.0: The Universal Forecaster Evolution"

    Published: August 2025

    Significance: Building on the original MOIRAI (the model for which LOTSA was created), version 2.0 expands the universal forecasting architecture to better handle messy, real-world data (MachineLearningMastery, 2026). It remains one of the primary models natively trained on the full 27-billion-observation LOTSA archive to achieve superior zero-shot generalization (Salesforce AI Research, 2025).

3. "TsLLM: Augmenting LLMs for General Time Series Understanding and Prediction"

    Published: October 2025 (Updated March 2026)

    Significance: This research focuses on reprogramming Large Language Models (LLMs) for time series tasks. It utilizes LOTSA as the large-scale pre-training corpus to align LLM embeddings with temporal patterns, enabling the model to perform both "Contextual Forecasting" and "Time Series Question-Answering" (Afrasiabi et al., 2025).

4. "OATS: Online Data Augmentation for Time Series Foundation Models"

    Published: January 2026

    Significance: This paper addresses the limitations of static datasets like LOTSA by introducing Online Data Augmentation (OATS). The authors use LOTSA as the baseline pre-training dataset to demonstrate how dynamic augmentation can further improve the robustness and cross-domain learning of foundation models (Liu et al., 2026).

5. "TSAQA: Time Series Analysis Question And Answering Benchmark"

    Published: January 2026

    Significance: While primarily a benchmark paper, it utilizes the diverse domains within the LOTSA archive (Finance, Healthcare, Energy, etc.) to construct a 210,000-sample dataset for evaluating whether AI models can "reason" about time series data rather than just predicting numbers (Brigato et al., 2026).

References

Brigato, L., et al. (2026). It's TIME: Towards the next generation of time series forecasting benchmarks. arXiv preprint. https://arxiv.org/html/2602.12147v1
MachineLearningMastery. (2026). The 2026 time series toolkit: 5 foundation models for autonomous forecasting. https://machinelearningmastery.com/the-2026-time-series-toolkit-5-foundation-models-for-autonomous-forecasting/
Salesforce AI Research. (2025). Moirai-2.0-R-small release. https://github.com/SalesforceAIResearch/uni2ts
TsLLM Team. (2025). TsLLM: Augmenting LLMs for general time series understanding and prediction. arXiv preprint. https://arxiv.org/html/2510.01111v2
Liu, X., et al. (2026). OATS: Online data augmentation for time series foundation models. arXiv preprint. https://arxiv.org/html/2601.19040v1
Woo, G., Liu, C., Sahoo, D., Kumar, A., & Hoi, S. (2024). Unified training of universal time series forecasting transformers. ICML 2024 Oral. https://doi.org/10.48550/arXiv.2402.02592
