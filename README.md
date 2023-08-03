# Similarity Project

Overall, in this project, we first consider multiple types of embeddings such as ComplEx, Transe, Abstract, Lexicalized embeddings and so on. Then, we use different sets of basis datasets for retrofitting these embeddings (bringing the neighbouring nodes closer to each other). We then evaluate the original and retrofitted embeddings on various evaluation benchmark datasets.

All the server files are uploaded on Google Drive [here](https://drive.google.com/drive/folders/1T-dE2tzF6iZDcDnaAmJeWERV-d3QwAk8?usp=sharing)

## Final GDrive Datasets and Results

Most of the results mentioned in the paper are derived from csv sheets generated from the Retrofitting notebook. The final versions of these results sheets can be found on Google Drive [here](https://drive.google.com/drive/folders/1akHrElVef2JJS7_m3oWxtSlqAISceIAY?usp=sharing)

Other files used can be found here:

* [Embedding Datasets](https://drive.google.com/drive/folders/1W7S-v2vVKHyLTqi3cgxiOJR7-_c2LG5j?usp=sharing) - Ignore the files in the folders
* [Basis Datasets](https://drive.google.com/drive/folders/19poqPcXbLjSl5PbYogMVUWneiRb-81XO?usp=sharing)
* [Evaluation Benchmark Datasets](https://drive.google.com/drive/folders/1_u2MqXzBiUSMPjWH5GRmp7RP2FUYYxf1?usp=sharing)

## [Embeddings Generation](https://github.com/usc-isi-i2/wd-similarity/blob/main/Embeddings%20Generation.ipynb)

In this notebook, we generate embeddings using ComplEx, Transe, lexicalized properties, abstract, H, A, S, labels only, labels + descriptions, and concatenated embeddings. In this notebook, we also generate direct similarity scores for pairs of nodes in evaluation benchmark datasets based on class, JC, topSim for direct evaluation in the Retrofitting notebook.

## [Basis Datasets Generation](https://github.com/usc-isi-i2/wd-similarity/blob/main/Basis%20Datasets%20Generation.ipynb), [Probase File Exploration](https://github.com/usc-isi-i2/wd-similarity/blob/main/Probase%20File%20Exploration.ipynb)

In the basis notebook, we generate the basis datasets using 2 relations - parent-child and siblings which we will later use in the Retrofitting notebook. In the probase notebook, we generate another such basis dataset.

## [Evaluation Datasets](https://github.com/usc-isi-i2/wd-similarity/blob/main/Evaluation%20Datasets%20Generation.ipynb)

In this notebook, we generate the evaluation benchmark datasets on which we evaluate our embeddings performance based on similarity both before and after retrofitting wherever applicable. We generate benchmarks for Wordsim353 (Annotated), DBPedia sourced datasets (MC 30, RG 65), ConceptNet, Wiki-CS but go on to using Wordsim and DBPedia ones only in the Retrofitting notebook. In the [ConcepNet Evaluation Dataset Exploration notebook](https://github.com/usc-isi-i2/wd-similarity/blob/main/ConceptNet%20Evaluation%20Dataset%20Exploration.ipynb), we just explore the ConceptNet dataset downloaded but the main file generation for our evaluation purpose is done in the main Evaluation Datasets notebook.

## [Retrofitting using Master Datasets](https://github.com/usc-isi-i2/wd-similarity/blob/main/Retrofitting%20using%20Master%20datasets.ipynb)

This is the main framework code where all the retrofitting, evaluation is done and results are captured.

Datasets Used:

* [Source ConceptNet File](https://drive.google.com/file/d/1bhkeTjDeheLXQdRpaJk6F5uTUFTpgQW0/view?usp=sharing)
* [Source Wiki-CS File](https://zenodo.org/record/3983030/files/wikidata-cs-20200504.tsv?download=1)
* [Source Probase Dataset](https://concept.research.microsoft.com/Home/Download)
* [DBPedia Abstracts Dataset](https://downloads.dbpedia.org/repo/dbpedia/text/short-abstracts/2020.07.01/short-abstracts_lang=en.ttl.bz2)
* [Wikidata DWD v2](https://drive.google.com/drive/u/3/folders/1OIZegxxrs_Hv2ZhDsSO-zLVARCR60P01)
* [Sitelinks from Wikidata 2020-12-08](https://drive.google.com/drive/u/3/folders/1qbbgjo7pddMdDvQzOSeSaL6lYwj_f5gi)
* [Wikidata Sibling and Child-Parent Data](https://drive.google.com/drive/u/1/folders/19poqPcXbLjSl5PbYogMVUWneiRb-81XO)

Project Draw.IO files stored on Google Drive [here](https://drive.google.com/drive/u/3/folders/1T4NrMo7TxroIq5flWBWL5nAaFm6-XWwb)
