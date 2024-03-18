# Introduction
This repo contains links to the eight datasets we generated for use in the NAS Unseen Data Challenges, held at the Neural Architecture Workshop at CVPR 2021, 2022, and 2023. We also show benchmark results to compare against in future works.

For a more detailed description of these datasets, please refer to out paper, accepcted at CVPR 2024:

Link Coming soon.

# Datasets
Below we will briefly describe and link to each dataset.

## AddNIST
<img src="./Images/AddNIST_single.svg" alt="Example of AddNIST" width="500">


AddNIST is generated by combining three MNIST Images. Each image is given a label which is the sum of the three sub-images minus one. In the above example the label would be 14. (((2 + 9 + 4) - 1) = 14).

The labels are limited between 0 - 19, giving a total of 20 classes. The dataset can be found at [data.ncl.ac.uk/articles/dataset/AddNIST_Dataset/24574354](https://data.ncl.ac.uk/articles/dataset/AddNIST_Dataset/24574354)

## Language
<img src="./Images/Language_single.svg" alt="Example of Language" width="500">

The language dataset is constructed using the ASPELL dictionary to collect words from multiple languages. Ten languages were chosen (English, Dutch, German, Spannish, French, Portuguese, Swedish, Zulu, Swahili, and Finnish).

The example above shows an image generated using the English label. Four words were chosen randomly from ASPELL (Uvulas, minted, suckle, and debits) and encoded into a 24x24 image. The y-axis depicts the character position in the concatenated 24-character string, and the x-axis represents the corresponding letter. For simplicity, words containing diacritics, or the letters 'y' and 'z' were removed before selection.

The dataset can be found at [data.ncl.ac.uk/articles/dataset/Language_Dataset/24574729](https://data.ncl.ac.uk/articles/dataset/Language_Dataset/24574729)

## MultNIST
<img src="./Images/MultNIST_single.svg" alt="Example of MultNIST" width="500">

Similar in design to AddNIST, MultNIST is also made up of three MNIST images. Instead of performing a summation, MultNIST labels are generated by multiplying the three sub-images together and performing a mod 10 operation on the result, which results in ten possible labels 0-9. In the example above the label would be 5. ((5 * 7 * 1) = 35. 35 mod 10 = 5).

The dataset can be found at [data.ncl.ac.uk/articles/dataset/MultNIST_Dataset/24574678](https://data.ncl.ac.uk/articles/dataset/MultNIST_Dataset/24574678)

## CIFARTile
<img src="./Images/CIFARTile_single.svg" alt="Example of CIFARTile" width="500">

CIFARTile is comprised of four CIFAR-10 images. The label of a CIFARTile image denotes how many unique CIFAR-10 labels from the sub-images are in the Image (i.e. a label of 0 means all four sub-images belong to the same CIFAR-10 class). This means there can be four labels, with a label of 3 denoting all sub-images belong to different classes.

The dataset can be found at [data.ncl.ac.uk/articles/dataset/CIFARTile_Dataset/24551539](https://data.ncl.ac.uk/articles/dataset/CIFARTile_Dataset/24551539)

## Gutenberg
<img src="./Images/Gutenberg_single.svg" alt="Example of Gutenberg" width="500">

Gutenberg is encoded similarly to Language, however, instead of representing words from different languages, Gutenberg encodeds three words extracted from public domain texts from Project Gutenberg (Note. these works are in the public domain in the US, please check your countries copyright law, before downloading).

The dataset can be found at [data.ncl.ac.uk/articles/dataset/Gutenberg_Dataset/24574753](https://data.ncl.ac.uk/articles/dataset/Gutenberg_Dataset/24574753)

## GeoClassing
![Example of GeoClassing](./Images/GeoClassing_single.svg)

The dataset can be found at [data.ncl.ac.uk/articles/dataset/GeoClassing_Dataset/24050256](https://data.ncl.ac.uk/articles/dataset/GeoClassing_Dataset/24050256)

## Isabella
![Example of Isabella](./Images/Isabella_single.svg)
Code Coming Soon.

## Chesseract
![Example of Chesseract represented in 2D](./Images/Chesseract_3d-2d.svg) ![The same example represented in 3D](./Images/Chesseract_3d.svg)

The dataset can be found at [data.ncl.ac.uk/articles/dataset/Chesseract_Dataset/24118743](https://data.ncl.ac.uk/articles/dataset/Chesseract_Dataset/24118743)

# Generation
You can find the code to generate five of the eight datasets at [github.com/RobGeada/cvpr-nas-datasets](https://github.com/RobGeada/cvpr-nas-datasets). We plan on releasing the code for generating the other datasets soon.

# Baseline Results

## CNN Results

## NAS Results

## Competition Results

## 2023 Top five finalists

## Best Competition Results

# Reference
Coming Soon

# License
<p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/Towers-D/NAS-Unseen-Datasets">NAS Unseen Datasets</a> by <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="http://davidtowers.uk">David Towers, Rob Geada, Amir Atapour-Abarghouei, Stephen McGough</a> is licensed under <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC BY 4.0<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"></a></p>