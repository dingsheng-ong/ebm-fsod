# Addressing Background Misclassification in Few-Shot Object Detection with Energy-Based Compositional Inference

## Abstract
> This paper revisits few-shot object detection (FSOD), focusing on how effectively object detectors learn novel objects from few labeled examples. While recent methods have achieved incremental improvements by introducing complex architectures, we reveal a fundamental problem rooted in the conventional two-stage fine-tuning framework, i.e., novel objects are often mislabeled as background in the base training stage. This mislabeling causes the base classifier to learn a biased distribution that conflates true background with novel objects, and this bias persists after fine-tuning, reducing detection accuracy on novel classes. In this work, we propose an approach to approximate the true background distribution alongside novel categories by estimating the intersection of distributions learned by both base and novel classifiers. Drawing on recent advances in energy-based models (EBMs), we reformulate the classifier of an object detector as an EBM, leveraging EBMs' compositional properties to derive more precise distributions for background and novel categories. Extensive experiments validate that our method consistently improves detection accuracy of the baseline model across benchmarks, including Pascal VOC and COCO.

Please use the provided script `display_results.py` to summarize and present the training logs:
```bash
usage: This script processes the results and formats them into a table. By providing the path to the checkpoint directory, the script will extract all the results found in the directory and store the table in csv format in the same directory.

Example:
    $ display_results.py checkpoints/voc/baseline

    This command will produce the table and save to:
    checkpoints/voc/baseline/results.txt

       [-h] [-v] [-s [SEED [SEED ...]]] path

positional arguments:
  path

optional arguments:
  -h, --help            show this help message and exit
  -v, --verbose
  -s [SEED [SEED ...]], --seed [SEED [SEED ...]]
```
