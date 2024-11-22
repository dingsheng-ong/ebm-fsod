# Addressing Background Misclassification in Few-Shot Object Detection with Energy-Based Compositional Inference

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
