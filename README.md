# Transfer Learning on CIFAR

This project compares several transfer-learning paths for image classification on CIFAR datasets. I built it to test when pretrained representations actually help and when training from scratch is still competitive.

The notebook covers four setups. It starts with a from-scratch CNN baseline on CIFAR10. It then compares ImageNet to CIFAR10 transfer, Places365 to CIFAR10 transfer, and a staged ImageNet to CIFAR100 to CIFAR10 path. I kept the evaluation structure consistent across the runs so the comparison stayed fair.

The main metrics are Top-1 accuracy and macro-F1. I also included learning curves and confusion matrices so the results are easier to interpret than just looking at a final score.

## Files

- `transfer_learning_on_cifar.ipynb` contains the full experiment pipeline
- `preview.jpg` is the visual I used for the portfolio site

## Tools

- Python
- PyTorch
- torchvision
- scikit-learn
- matplotlib
- seaborn

## Running the Project

1. Create an environment and install the packages in `requirements.txt`.
2. Open `transfer_learning_on_cifar.ipynb` in Jupyter or Colab.
3. Run the notebook from top to bottom.
4. Let the setup cells download the required datasets or pretrained weights if they are not already available.

## What This Project Shows

- transfer learning under multiple training paths instead of a single baseline comparison
- controlled experiment design with aligned metrics and evaluation
- practical model analysis using accuracy, macro-F1, curves, and confusion matrices

## Notes

- Some sections take time because the project includes repeated training and comparison runs.
- If I publish a later revision, I would add a compact final-results table and saved checkpoints.
