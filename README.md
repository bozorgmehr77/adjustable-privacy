# adjustable-privacy
The Implementation Code of Journal Paper (Adjustable Privacy using Autoencoder-based Learning Structure)

All of these codes are written in Jupyter Notebook.
For simplicity, clone this repository into your google drive and use google colab.

Guide:

1- Clone the directory to the root of your google drive.

2- Add a shortcut to this shared CelebA directory in "adjustable-privacy\Datasets" with the "CelebA" name:
https://drive.google.com/drive/folders/0B7EVK8r0v71pWEZsZE9oNnFzTm8?resourcekey=0-5BR16BdXnb8hVj6CNHKzLg&usp=share_link

- NOTE: All parameter sets for loading pre-trained models are available in "parameter set for loading models.txt"
- NOTE: For more detail about each notebook, read the embedded comments in that notebook.

(In image dataset case:)

3- (Image Case\train_on_original.ipynb) To train a network (for example, weak adversary) on the original dataset (to infer a specific feature), simply set the parameters of the parser and run the notebook. Also, you can load our pre-trained models and see the results.

4- (Image Case\train_obfuscator.ipynb) To train or load the obfuscator, set parser parameters and run this notebook.

5- (Image Case\create_obfuscated_dataset.ipynb) To obfuscate a dataset, use this notebook. It creates a zip file of the obfuscated dataset on your google drive.

6- (Image Case\train_on_obfuscated.ipynb) You can use this notebook to train a network (utilizer or strong adversary) on the obfuscated dataset. Also, it evaluates weak adversary on the obfuscated dataset.

(In categorical dataset case:)

3- (Categorical Case\train_on_original.ipynb) To train a network (for example, weak adversary) on the original dataset (to infer specific feature).

4- (Categorical Case\train_obfuscator.ipynb) To train or load obfuscator.

5- (Categorical Case\create_obfuscated_dataset_and_train_on.ipynb) This notebook creates obfuscated data and trains a network on it (utilizer or strong adversary)

(Others)

- (Others\model_number_and_lambda_selection.ipynb) This file investigates the impact of the model number and lambda on the utility privacy trade-off.
- (Others\decorrelation_test.ipynb) This file is used to prove the decorrelation of utility features from others.
- (Others\plots_of_image_case.ipynb) This file contains utility privacy trade-off plots in the image case.
- (Others\plots_of_categorical_case.ipynb) This file contains utility privacy trade-off plots in the categorical case.
