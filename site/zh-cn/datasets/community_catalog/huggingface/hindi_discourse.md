# hindi_discourse

参考：

- [代码](https://github.com/huggingface/datasets/blob/master/datasets/hindi_discourse)
- [Huggingface](https://huggingface.co/datasets/hindi_discourse)

使用以下命令在 TFDS 中加载此数据集：

```python
ds = tfds.load('huggingface:hindi_discourse')
```

- **说明**：

```
The Hindi Discourse Analysis dataset is a corpus for analyzing discourse modes present in its sentences.
It contains sentences from stories written by 11 famous authors from the 20th Century.
4-5 stories by each author have been selected which were available in the public domain resulting
in a collection of 53 stories. Most of these short stories were originally written in Hindi
but some of them were written in other Indian languages and later translated to Hindi.
```

- **许可**：无已知许可
- **版本**：1.0.0
- **拆分**：

拆分 | 样本
:-- | --:
`'train'` | 9968

- **特征**：

```json
{
    "Story_no": {
        "dtype": "int32",
        "id": null,
        "_type": "Value"
    },
    "Sentence": {
        "dtype": "string",
        "id": null,
        "_type": "Value"
    },
    "Discourse Mode": {
        "num_classes": 6,
        "names": [
            "Argumentative",
            "Descriptive",
            "Dialogue",
            "Informative",
            "Narrative",
            "Other"
        ],
        "names_file": null,
        "id": null,
        "_type": "ClassLabel"
    }
}
```
