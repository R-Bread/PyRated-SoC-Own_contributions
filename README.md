# PyRated-SoC-Own_contributions

## Summer of Code project - PyRated

## - Plagiarism detector for c++ files

# Own contributions

This repository contains the code I wrote for my 2021 Summer of Code project, in team PyRated, at IITB. For the complete project, please click here.

NOTE: Few of these code files will work on their own - most import from other files only present in the complete project repository.

All code files I wrote are in Python - c++ files are the dataset to test on.



# .exe Comparison

exe_comparison.py is one of the plagiarism testing functions of the project and was  written by me. It takes in the addresses of two files compile them and compares the compiled .out files, and outputs a percentage match.



# Final Code

Contains the file Multi_Layer_Comparison.py, which contains the final function which takes in two c++ code files and outputs true or false accordingly. It can also output a list or dictionary of the percentage matches from each test function.

It imports the test functions from other files which are not present in this repository. 

Part of the code in this file such as the key result function and the optional argument processing, and the with statements and try-except loops - to ensure smooth running despite errors or problems in the files - were written by me.



# Test Dataset

dataset_testing.py goes through the data set, feeds each pair to the multiLayerComparison function from Multi_Layer_Comparison.py, and using a file called truth.txt, which lists the plagiarised sets, prints how well the main function and each individual testing function performed.



# Plotting Results

plotting.py also goes through the data set, feeds each pair to each of the individual testing functions, and using matplotlib and numpy it creates a scatter plot showing what percentage matches plagiarised and non-plagiarised pairs show. This helps in determining the ideal threshold for these functions in the main function.



# Results

Contains a few screenshots of the results obtained by me.



# Code Pruning

Initially written to remove comments and unused functions from python and c++ code files (for Python as well, because initially we had planned to write the detector for Python). Not directly imported anymore, but the regex code from this was directly used in the final project result.
