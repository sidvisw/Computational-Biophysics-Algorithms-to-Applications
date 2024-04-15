# Implementing miRNA-mRNA Interaction Prediction from miRNA-mRNA Interaction Graph

This project aims to implement a basic GNN based prediction algorithms on miRNA-mRNA interaction prediction from the miRNA-mRNA interaction graph.

The steps involved in this project are as follows:

## 1. Download and Extract the RNA-RNA Interaction Database

The RNA-RNA interaction database can be downloaded from the following link: [RNAInter Database](http://www.rnainter.org/raidMedia/download/Download_data_RR.tar.gz).

## 2. Filter the Database

Filter the database for the species 'Homo sapiens', Category1 as 'miRNA', and Category2 as 'mRNA'.

## 3. Select Rows and Find the Largest Connected Component from the Interaction Graph

Select any 50000 rows from the filtered dataset and find the largest connected component from the resulting graph.

## 4. Train an Edge Prediction Algorithm (GNN)

Divide the edges into train and test sets and train any edge prediction algorithm. A basic Graph Neural Network (GNN) with randomly initialized nodes is used in our case.

## 5. Report the Results

Finally, report the results like Mean Squared Error, Mean Absolute Error, R-squared score, etc.

## Steps to run the Jupyter Notebook (main.ipynb)

1. Download and extract the RNA-RNA Interaction Database.

```
# Download command
wget http://www.rnainter.org/raidMedia/download/Download_data_RR.tar.gz

# Extracting the file
tar -xvzf Download_data_RR.tar.gz
```

2. Create a python virtual environment and install all the required packages.

```
# Creating a virtual environment
python3 -m venv .venv
source .venv/bin/activate

# Installing all the required dependencies
pip install -r requirements.txt
```

3. Now, select the virtual environment created while running the Jupyter Notebook (main.ipynb).

Please refer to the main.ipynb file for the complete code and detailed implementation.

## Authors and Contributors

- [Sidharth Vishwakarma - 20CS10082](https://github.com/sidvisw)
- [Grace Sharma - 20CS30022](https://github.com/Grce47)
- [Vineet Amol Pippal - 20CS30058](https://github.com/vaptheone)
