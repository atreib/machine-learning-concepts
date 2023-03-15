# Pre-processing

## Importing your dataset

When working with CSV, we can use panda's `read_csv()` function, as the following example:

```
import pandas as pd
my_dataset = pd.read_csv("path/to/file.csv")
```

When reading a CSV, you may have some specific necessities. You may or not have a header row. You may or not want to name your columns... So `read_csv()` have some amazing arguments that you can use. Look at the code below:

```
import pandas as pd
col_names = ['channel', 'watch_time', 'stream_time', 'peak_viewers', 'average_viewers', 'followers', 'followers_gained', 'views_gained', 'is_partner', 'is_mature', 'language']
dataset = pd.read_csv("input/twitchdata-update.csv", skiprows=1, header=None, names=col_names)
```

As you can see, we have an array with our columns' names and passing it to the `names` argument.
Also, we are passing `skiprows=1`, and, by doing that, we are skipping the header row of the CSV file.

## Analyzing your dataset

After loading your dataset, here's a few cool methods to use:

```
my_dataset.head() # load the first few records from the dataset
my_dataset.describe() # !!! gets average, max, min, and other cool info about the dataset
```
