This repository provides the datasets for the paper "Finding Truth in the Sea of Opinions: Using Large Language Models for Fake Review Detection" handed in to ECIR 2027. The datasets can be found in the subfolder data.

The LLM generators used were:
- **Small:** Gemma 4 (E4B), Ministral 3 (8B), Llama 3.2 (3B), Qwen 3.5 (9B)
- **Large:** DeepSeek-V4-Flash, GLM-5.3-Flash, GPT 5.6 Luna, GPT 5.6 Terra

### Datasets

| dataset | test n | Generator | floor | human real | human fake | synthetic |
|---|---|---|---|---|---|
| `d1_human_real_vs_human_fake` | 398 | -- | 0.500 | 199 | 199 | 0 |
| `d2_sampled_human_real_vs_synthetic` | 398 | Small | 0.500 | 199 | 0 | 199 |
| `d2.5_sampled_human_real_vs_synthetic` | 398 | Large | 0.500 | 199 | 0 | 199 |
| `d2.5_unsampled_human_real_vs_synthetic` | 679 | Large | 0.707 | 199 | 0 | 480 |
| `d3_sampled_human_real_vs_mixed` | 398 | Small | 0.500 | 199 | 99 | 100 |
| `d3_unsampled_human_real_vs_mixed` | 598 | Small | 0.667 | 199 | 199 | 200 |
| `d3.5_sampled_human_real_vs_mixed` | 398 | Large | 0.500 | 199 | 99 | 100 |
| `d3.5_unsampled_human_real_vs_mixed` | 878 | Large |0.773 | 199 | 199 | 480 |

Note: d1 is essentially the Deceptive Opinion Spam Corpus with our training-test split.

### Citation

Ott, M., Choi, Y., Cardie, C., Hancock, J.T.: Finding deceptive opinion spam by any stretch of the imagination. In: Lin, D., Matsumoto, Y., Mihalcea, R. (eds.) Proceedings of the 49th Annual Meeting of the Association for Computational Linguistics: Human Language Technologies. pp. 309–319. Association for Computational Linguistics, Portland, Oregon, USA (Jun 2011), https://aclanthology.org/P11-1032/