# Understanding the Benefits of Forgetting when Learning on Dynamic Graphs

		 
## PREAMBLE

This work was published at ECML-PKKD 2022. It was funded by the IMPULSION 
program as part of the IDEX from Université De Lyon (UDL) 

## ABOUT

This repository contains source code to learn node embeddings for dynamic 
networks.  It  also  contains  some  scripts  to evaluate the performances of the 
node embeddings on the tasks of node classification and edge prediction.    

Related paper can be found   at  xxx.

If you use this repository, please cite:

	@inproceedings{tissier2022Dyn,
	  author    = {Tissier, Julien and Laclau, Charlotte},
	  title     = {Understanding the Benefits of Forgetting when Learning on Dynamic Graphs},
	  booktitle = {Proceedings of ECML-PKDD},
	  volume    = {},
	  pages     = {},
	  year      = {2022},
	}

## INSTALLATION

To be able to run the experiments, you will need:
    - Python 3.8

This code works only with Python 3.8 (and not with later version) because one
of the Python library we use does not support Python 3.9+.
To install Python3.8 on you machine, you can use the following link:
    https://www.python.org/downloads/release/python-387/

Then, install the dependencies with the following commands:

    1) python3.8 -m venv ~/Dynamic-env
    2) source ~/Dynamic-env/bin/activate
    3) python3.8 -m pip install -r requirements.txt


## DOWNLOADING MISSING DATASETS

Due to its size, we could not include the dataset Subreddit inside this
supplementary (however, all the other datasets are provided in this folder).
To download it, run the following command inside the same folder as this README:

wget https://snap.stanford.edu/data/soc-redditHyperlinks-body.tsv -P datasets/

To evaluate on the node classification task, you will also need FastText
pretrained word vectors. You can download them at the following URL:

https://dl.fbaipublicfiles.com/fasttext/vectors-wiki/wiki.en.zip

Then, extract the zip file and move the file "wiki.en.bin" inside the datasets/
directory of this folder.

## AUTHOR

	The code was written  by  Julien  Tissier  <30314448+tca19@users.noreply.github.com>.

## COPYRIGHT

	This software is licensed under the GNU GPLv3 license.  See the  LICENSE
	file for more details.
