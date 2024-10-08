# bc2gm_corpus

参考：

- [代码](https://github.com/huggingface/datasets/blob/master/datasets/bc2gm_corpus)
- [Huggingface](https://huggingface.co/datasets/bc2gm_corpus)

## bc2gm_corpus

使用以下命令在 TFDS 中加载此数据集：

```python
ds = tfds.load('huggingface:bc2gm_corpus/bc2gm_corpus')
```

- **说明**：

```
Nineteen teams presented results for the Gene Mention Task at the BioCreative II Workshop.
In this task participants designed systems to identify substrings in sentences corresponding to gene name mentions.
A variety of different methods were used and the results varied with a highest achieved F1 score of 0.8721.
Here we present brief descriptions of all the methods used and a statistical analysis of the results.
We also demonstrate that, by combining the results from all submissions, an F score of 0.9066 is feasible,
and furthermore that the best result makes use of the lowest scoring submissions.

For more details, see: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2559986/

The original dataset can be downloaded from: https://biocreative.bioinformatics.udel.edu/resources/corpora/biocreative-ii-corpus/
This dataset has been converted to CoNLL format for NER using the following tool: https://github.com/spyysalo/standoff2conll
```

- **许可**：无已知许可
- **版本**：1.0.0
- **拆分**：

拆分 | 样本
:-- | --:
`'test'` | 5001
`'train'` | 12501
`'validation'` | 2501

- **特征**：

```json
{
    "id": {
        "dtype": "string",
        "id": null,
        "_type": "Value"
    },
    "tokens": {
        "feature": {
            "dtype": "string",
            "id": null,
            "_type": "Value"
        },
        "length": -1,
        "id": null,
        "_type": "Sequence"
    },
    "ner_tags": {
        "feature": {
            "num_classes": 3,
            "names": [
                "O",
                "B-GENE",
                "I-GENE"
            ],
            "names_file": null,
            "id": null,
            "_type": "ClassLabel"
        },
        "length": -1,
        "id": null,
        "_type": "Sequence"
    }
}
```
