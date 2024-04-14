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

Due to a lack of benign data (as seen in the baseline experiment), more data
was captured on a local machine (macOS) using
[PacketLogger](https://www.bluetooth.com/blog/a-new-way-to-debug-iosbluetooth-applications/),
then it was exported to `.btsnoop` format and converted to `.csv` format using
Wireshark. The captured data is available
[here](https://www.icloud.com/iclouddrive/031kzui9eqKLht9L8aIDuukIQ#capture).
The resulting dataset files are:

- `data/capture.csv`

The data was captured with the following devices connected via Bluetooth:

- Headphones
- AirPods
- Mouse
- Game controller
- Smartwatch

## Experiments

Each experiment done is run is a separate Jupyter notebook. The notebooks are
stored in the `notebooks` directory. An experiment's notebook outlines the
experiment's purpose and findings. The notebook contains the results of the
experiment through text and visualizations.
