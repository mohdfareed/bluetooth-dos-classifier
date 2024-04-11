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

## Experiment Tracking

Tracking is done through logging to a file. The logs are stored in the
`experiments` directory. Each experiment is stored in a separate file. All
generated models are stored in the `models` directory, with the experiment
number appended to the filename.

This allows for easy tracking of experiments, their results, and the models
generated by each experiment. It requires the notebook to log all relevant
experiment information. If plots are generated, they will be stored with the
experiment number also appended to the filename.
