# MNIST AI Notebook

This project contains a TensorFlow/Keras notebook for training and testing a CNN on the MNIST handwritten digits dataset.

Notebook file:
- `MNIST_AI.ipynb`

## What The Notebook Does

- Imports ML and visualization libraries.
- Loads MNIST data and prints dataset sizes.
- Builds a CNN model (`Conv2D -> MaxPool -> Conv2D -> MaxPool -> Flatten -> Dense -> Dense`).
- Trains for 3 epochs.
- Predicts one random test image.
- Plots training/validation accuracy and loss.
- Saves model architecture and weights.
- Loads saved model back from disk.
- Evaluates test performance.

## Requirements

Install Python packages before running:

```bash
pip install tensorflow numpy matplotlib scikit-learn opencv-python
```

## How To Run

1. Open `MNIST_AI.ipynb` in VS Code or Jupyter.
2. Select a Python environment with the required packages installed.
3. Run cells in order from top to bottom (Cell 1 through Cell 11).

## Output Files Generated

After running the notebook, these files are created in the same folder:
- `img_model.png` (model architecture diagram)
- `model.json` (model architecture in JSON)
- `model.weights.h5` (trained model weights)

## Notes

- First run may take longer because MNIST data is downloaded.
- Training time depends on hardware.
- If `plot_model` fails, install Graphviz and ensure it is available in your system path.

## Troubleshooting

- `ModuleNotFoundError`: install missing packages from the Requirements section.
- TensorFlow installation issues on Windows: upgrade `pip` and reinstall TensorFlow.
- If a cell errors, restart kernel and rerun all cells in order.
