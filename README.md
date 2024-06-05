# textannotate

textannotate is a local annotation tool for use in labeling text classification data. You can also use textannotate to check the labels of an existing dataset.

textannotate supports data in the jsonl format.

textannotate comes with several keyboard shortcuts to assist in annotation. You can use:

1. `1-9` to label with a number, where each number corresponds to a class in your dataset. These numbers are changed to the actual class names when you save the annotations.
2. `left arrow` and `right arrow` to move between records in your dataset.
3. `s` to show or hide any long description. This is useful if you are annotating a dataset with titles and descriptions where you decide you don't need to see the description to make a classification.

## How to Use

First, install textannotate:

```
pip3 install textannotate
```

Then, run the following command:

```
textannotate -f path/to/your/data.jsonl -c [name of class field] -d [name of description field]
```

Where:

- `path/to/your/data.jsonl` is the path to your dataset in jsonl format.
- `name of class field` is the name of the field in your dataset that contains the class label.
- `name of description field` is the name of the field in your dataset that contains the description.

textannotate will run on `localhost:5000`.

Every five annotations you make, textannotate automatically saves your results to your dataset.

## License

This project is licensed under an [MIT license](LICENSE).