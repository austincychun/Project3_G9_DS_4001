# Data Folder Documentation

This folder contains the datasets used for the analysis of artwork images. Below is the metadata and context required to interpret the data effectively.

## 1. Data Summary
The dataset consists of metadata and paths for a collection of artwork images, primarily sourced from Art UK. It is organized into two main CSV files:

* **`painting_dataset_2021.csv`**: The primary dataset containing 17,258 entries. It includes URLs to the original images, web page links, class labels (e.g., 'cow', 'train'), and data split assignments.
* **`images_with_paths_half.csv`**: A supplementary file containing 2,113 entries that maps a subset of images to their local file paths (`/scratch/$USER/images/...`) for training.

## 2. Provenance
* **Source:** Art UK (via University of Oxford Visual Geometry Group)
* **URL:** [https://artuk.org/](https://artuk.org/)
* **Collection Method:** Curated from the Art UK public collection.
* **Date Accessed:** November 5, 2025

## 3. License
The metadata is provided for educational and research purposes.
* **Usage:** Please refer to the specific copyright notices on [artuk.org](https://artuk.org/) for each image.
* **GitHub Repository License:** MIT License.

## 4. Ethical Statements
* **Bias & Representation:** The dataset relies on the Art UK collection, potentially centering on Western/European art traditions.
* **Copyright:** We respect the intellectual property of the artists. This repository stores metadata and scripts; high-resolution image files are not distributed directly.

## 5. Data Dictionary
**File: `painting_dataset_2021.csv`**
| Variable Name | Data Type | Description |
| :--- | :--- | :--- |
| `Image URL` | String | Direct URL to the image file. |
| `Web page URL` | String | URL to the artwork's page on Art UK. |
| `Subset` | String | Partition: `'train'`, `'test'`, or `'val'`. |
| `Labels` | String | Class label (e.g., `'cow'`). |

**File: `images_with_paths_half.csv`**
| Variable Name | Data Type | Description |
| :--- | :--- | :--- |
| `Local Path` | String | Absolute file path to the image stored locally. |
| *(Other columns match above)* | | |

## 6. Explanatory Plots

**Plot 1: Distribution of Subject Types**
As outlined in our analysis plan, we examined the dataset for class imbalance. The pie chart below (extracted from our MI2 report) illustrates the breakdown of the most common subject types.
<img width="766" height="790" alt="graph1" src="https://github.com/user-attachments/assets/f1dae627-da6b-4ae2-8bba-5f5dc544bafb" />


**Plot 2: Data Split Distribution**
This chart visualizes how the dataset is partitioned into training, testing, and validation sets.
<img width="794" height="504" alt="graph2" src="https://github.com/user-attachments/assets/e845108c-f110-4177-86c3-a26ea08e5c62" />

