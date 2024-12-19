# Data Description

### How to load the data
Our dataset is relatively large so we have compiled them inside `data.tar.gz`. Once you download and unzip all the files, the data should be divided into the train, dev, and test subsets that were used for this project.

### Data Collection & Generation

The fake review dataset contains 40,000 entries:

- **20,000 authentic (OR) reviews**: Human-written from the Amazon Reviews dataset.
- **20,000 fake (CG) reviews**: Generated using the GPT-2 language model, fine-tuned on Amazon’s review data.

For the generated reviews, the creators used stratified sampling across the Top-10 Amazon product categories, balancing various review lengths to align with the original data distribution.

We used an 80/10/10 training/development/testing split to partition the data.

### Data Fields

The dataset contains the following columns:

- **category**: Product category identifier (e.g., `Home_and_Kitchen_5`).
- **rating**: Product rating, from 1 to 5.
- **label**: Review type - "OR" for Original and "CG" for Computer-Generated.
- **text\_**: Full text of the review.

### Example Data

| category           | rating | label | text\_                                                                      |
| ------------------ | ------ | ----- | --------------------------------------------------------------------------- |
| Home_and_Kitchen_5 | 5.0    | CG    | Love this! Well made, sturdy, and very comfortable. I love it! Very pretty. |
| Books_5            | 4.0    | OR    | Good story. Good book. Jennifer Ryan consistently writes great books.       |

### File Format

The data is stored in CSV format with the following columns: `category`, `rating`, `label`, and `text_`, and in the following directories: `train`, `dev`, and `test`.

### Dataset Source

Salminen, J., Kandpal, C., Kamel, A. M., Jung, S., & Jansen, B. J. (2022). Creating and detecting fake reviews of online products. Journal of Retailing and Consumer Services, 64, 102771. https://doi.org/10.1016/j.jretconser.2021.102771

The dataset is linked at https://www.kaggle.com/datasets/mexwell/fake-reviews-dataset/data.
