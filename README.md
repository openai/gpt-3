# GPT-3: Language Models are Few-Shot Learners

[arXiv link](https://arxiv.org/abs/2005.14165)
> Recent work has demonstrated substantial gains on many NLP tasks and benchmarks by pre-training on a large corpus of text followed by fine-tuning on a specific task. While typically task-agnostic in architecture, this method still requires task-specific fine-tuning datasets of thousands or tens of thousands of examples. By contrast, humans can generally perform a new language task from only a few examples or from simple instructions – something which current NLP systems still largely struggle to do. Here we show that scaling up language models greatly improves task-agnostic, few-shot performance, sometimes even reaching competitiveness with prior state-of-the-art fine-tuning approaches. Specifically, we train GPT-3, an autoregressive language model with 175 billion parameters, 10x more than any previous non-sparse language model, and test its performance in the few-shot setting.  For all tasks, GPT-3 is applied without any gradient updates or fine-tuning, with tasks and few-shot demonstrations specified purely via text interaction with the model.  GPT-3 achieves strong performance on many NLP datasets, including translation, question-answering, and cloze tasks, as well as several tasks that require on-the-fly reasoning or domain adaptation, such as unscrambling words, using a novel word in a sentence, or performing 3-digit arithmetic. At the same time, we also identify some datasets where GPT-3's few-shot learning still struggles, as well as some datasets where GPT-3 faces methodological issues related to training on large web corpora. Finally, we find that GPT-3 can generate samples of news articles which human evaluators have difficulty distinguishing from articles written by humans.  We discuss broader societal impacts of this finding and of GPT-3 in general.

## Contents
- [175b_samples.jsonl](175b_samples.jsonl) - Unconditional, unfiltered 2048 token samples from GPT-3 with p=.85, t=1.&#12288;
**CONTENT WARNING:** GPT-3 was trained on arbitrary data from the web, so may contain offensive content and language.
- [data](data) - Synthetic datasets for word scramble and arithmetic tasks described in the paper.
- [dataset_statistics](dataset_statistics) - Statistics for all languages included in the training dataset mix.
- [overlap_frequency.md](overlap_frequency.md) - Samples of 13-gram overlaps between our training data and benchmarks, selected by frequency in the training set.
- [model-card.md](model-card.md) - GPT-3 Model Card.

## How to cite
```
@article{brown2020language,
    title={Language Models are Few-Shot Learners},
    author={Tom B. Brown and Benjamin Mann and Nick Ryder and Melanie Subbiah and Jared Kaplan and Prafulla Dhariwal and Arvind Neelakantan and Pranav Shyam and Girish Sastry and Amanda Askell and Sandhini Agarwal and Ariel Herbert-Voss and Gretchen Krueger and Tom Henighan and Rewon Child and Aditya Ramesh and Daniel M. Ziegler and Jeffrey Wu and Clemens Winter and Christopher Hesse and Mark Chen and Eric Sigler and Mateusz Litwin and Scott Gray and Benjamin Chess and Jack Clark and Christopher Berner and Sam McCandlish and Alec Radford and Ilya Sutskever and Dario Amodei},
    year={2020},
    eprint={2005.14165},
    archivePrefix={arXiv},
    primaryClass={cs.CL}
}
```
