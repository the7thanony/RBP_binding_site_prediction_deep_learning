RNA-Protein Binding Site Prediction using Deep Learning
Overview
This project leverages Convolutional Neural Networks (CNNs) to predict RNA-binding protein (RBP) binding sites, focusing on AGO2, a protein involved in microRNA-mediated gene silencing. By employing deep learning, the model eliminates the need for manual feature engineering, capturing complex patterns within RNA sequences. The project demonstrates how local and global sequence information can be integrated to enhance prediction accuracy.

Features
Predicts RBP binding sites using RNA sequence data.
Combines local and global sequence contexts for improved predictions.
Utilizes one-hot encoding for RNA sequences.
Implements regularization techniques (dropout, early stopping) for robust training.
Achieves ~75% accuracy on validation data.
Dataset
The dataset is sourced from the GraphProt database:

Positive and negative RNA sequences in FASTA format.
Training Set: 92,346 sequences.
Testing Set: 1,000 sequences.
Preprocessing includes one-hot encoding, padding, and formatting for CNN input.

Usage
Preprocessing the Dataset
Ensure your RNA sequences are in FASTA format.
Preprocess the data using the included Python scripts:
One-hot encoding: Converts nucleotides (A, C, G, U) to binary vectors.
Padding: Ensures uniform sequence length.

Results
Training Accuracy: ~85%.
Validation Accuracy: ~75%.
Test Accuracy: ~74%.
Visualization
Accuracy Plot: Training vs. Validation Accuracy

Loss Plot: Training vs. Validation Loss

Technologies Used
Python: Programming language.
TensorFlow/Keras: Deep learning framework.
Biopython: Parsing and handling biological sequence data.
NumPy: Data manipulation and preprocessing.
