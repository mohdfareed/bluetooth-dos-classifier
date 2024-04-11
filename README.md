# Bluetooth DoS Classifier

Classifier of Bluetooth packets to detect DoS attacks.

## Prerequisites

- Python 3.12

## Usage

Run the following to clone the repository and setup the environment.

```sh
git clone https://github.com/mohdfareed/bluetooth-dos-classifier.git
cd bluetooth-dos-classifier
./setup.sh
```

Open the Jupyter notebook and select the environment `.venv` as the kernel.

## Dataset

The dataset is obtained from the following link:
https://www.unb.ca/cic/datasets/iomt-dataset-2024.html

The specific dataset used is the "Bluetooth" dataset. The dataset is in `.pcap`
format. The dataset is first converted to `.csv` format using the `tshark`
command line tool (WireShark can also be used). The resulting dataset files
are:

- `data/benign_test.csv`
- `data/benign_train.csv`
- `data/dos_test.csv`
- `data/dos_train.csv`
