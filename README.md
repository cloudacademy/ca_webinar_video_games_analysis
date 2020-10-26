# Cloud Academy Webinar
# Title: Karting Through Video Games History with Python: how to manipulate your data from Zelda to CoD

## Speaker info
This webinar is held by Andrea Giussani, Data Scientist at Cloud Academy.
You can reach him out at [:email:](andrea.giussani@cloudacademy.com), and you can follow him either on his :rocket: [blog](https://andreagiussani.github.io/the-long-beard-blog/) or via [GitHub](https://github.com/andreagiussani).

## Setting Up the Google Colab Environment

The Google Colab is a product from Google Research which allows
> anybody to write and execute arbitrary python code through the browser, and is especially well suited to machine learning, data analysis and education. More technically, Colab is a hosted Jupyter notebook service that requires no setup to use, while providing free access to computing resources including GPUs.

For more information, please visit the following [link](https://research.google.com/colaboratory/faq.html).

Here, we provide a short tutorial on how to upload the data on that environemnt via Google drive, and then use the Google colab to run your analysis.
Please, note that we assume you have a google account to access to this Google product.

### 1. Open a Google Colab session

From your favourite browser, open a new colab notebook via the following [link](https://colab.research.google.com)

### 2. Mount your drive on colab

I am assuming you have placed the data into the `My Drive` folder. If so, connecting your drive to a google machine is pretty easy, using the python google library: just run the following code snippet:

```python
from google.colab import drive
drive.mount('/content/drive')
```
after an authorisation check, you will be able to interact with your drive content either from the file browser side panel (easier) or using command-line utilities.

### 3. Let's get our hands dirty
Just run the following snippet to put the raw data into a pandas dataframe:
```python
import pandas as pd
df = pd.read_csv('/content/drive/My Drive/<FILENAME>.csv')
```
Are you ready? Let us get started!
