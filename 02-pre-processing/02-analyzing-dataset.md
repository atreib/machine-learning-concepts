# Pre-processing

## Analyzing your dataset

After loading your dataset, a good next step is to understand your dataset, trying to find issues. A few broken features may mislead your trained model.

Here are a few cool methods you can use:

```
my_dataset.head(10) # loads the first 10 records from the dataset
my_dataset.tail(10) # loads the last 10 records from the dataset
my_dataset.describe() # !!! gets average, max, min, and other cool statistics about the dataset
```

> Kudos for the `describe()` method. It can help you to find null values and some other important things :)

Tag with the describe findings to go directly to some records. Look at the code below:

```
my_dataset[my_dataset['col_name'] >= 120]
```

This line of code is going to return the filter of your dataset. It can be very helpful to analyze it.
