# 🚦 FiftyOne Workshop: Mobility Edition 
## Pre-Workshop Preparation

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1_eqFf8E4gC42y7oipX6BmNi_dJz-MfVv)

Welcome to the **FiftyOne Mobility Workshop**!  
To get the most out of the session, please follow the preparation steps below.


## Things To Do **One Day Before** the Workshop

### 1. Create a Hugging Face Account (**Mandatory**)
- Sign up at [huggingface.co](https://huggingface.co/join)
- Go to your [Access Tokens](https://huggingface.co/settings/tokens) and create a **Read token**


### 2. Optional but Highly Recommended Readings (📖)
These resources will give you a head start and make the workshop smoother:

- [Loading datasets from Hugging Face](https://docs.voxel51.com/integrations/huggingface.html#loading-datasets-from-the-hub)
- [Dataset Views (Filtering, Slicing, Searching)](https://docs.voxel51.com/user_guide/using_views.html)
- [Clustering with Embeddings](https://docs.voxel51.com/tutorials/clustering.html?highlight=embedding)
- [MosaicML Integration (Embeddings)](https://docs.voxel51.com/integrations/mosaic.html?highlight=embedding)
- [FiftyOne Plugins API](https://docs.voxel51.com/api/fiftyone.plugins.html?highlight=plugin#module-fiftyone.plugins)



### 3. Bonus Concept to Explore: **Embeddings**
We’ll explore this in detail during the session, but if you're curious:
- [CLIP Paper by OpenAI](https://arxiv.org/abs/2103.00020)



## ⏰ Task To Do **20 Minutes Before** the Workshop (Mandatory)

> This depends on your internet speed. It could take **10–25 minutes**. Please run the following **at least 20 minutes before the workshop** in Google Colab.

Just run the following cell in your Google Colab notebook:

```python
# THIS IS THE MINIMUM REQUIREMENT AFTER YOU INSTALL ALL THE DEPENDENCIES.
import os
import fiftyone.utils.huggingface as fouh
from huggingface_hub import login

login(token="ADD_YOUR_HF_TOKEN_HERE") 
dataset = fouh.load_from_hub("dgural/bdd100k", persistent=True, name="bdd100k_test")
````

Make sure to **replace** `"ADD_YOUR_HF_TOKEN_HERE"` with your Hugging Face token.



## 🏆 SUPER BONUS: Become an Open Source Contributor!

If you **find an issue in the docs** before the workshop, you’ll earn a **premium badge of honor** 😎

* Try to fix it yourself and submit a PR!
* Can’t fix it yet? **No worries!** Tell me during the workshop and I’ll guide you through your **first open-source contribution.**

Welcome to the cool club of contributors 🚀
