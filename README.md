# Deep Learning Fundamentals — NVIDIA DLI + PyTorch practice

My working notebooks from the **NVIDIA Deep Learning Institute "Fundamentals of Deep Learning"** course
(certificate of competency, December 2025) and the PyTorch practice I did alongside it.

The DLI notebooks follow the course labs; the `0x_pytorch_*` notebooks follow the open
[*Learn PyTorch for Deep Learning*](https://github.com/mrdbourke/pytorch-deep-learning) curriculum
(Zero to Mastery, Daniel Bourke), which I used to rebuild the same ideas in plain PyTorch.
Course material belongs to its authors; the code cells and experiments are mine.

## NVIDIA DLI — Fundamentals of Deep Learning

| Notebook | Topic |
|---|---|
| `00_jupyterlab.ipynb` | Lab environment |
| `01_mnist.ipynb` | First image classifier on MNIST: data loading, a fully connected network, training loop |
| `02_asl.ipynb` | American Sign Language letters with a dense network — and why it overfits |
| `03_asl_cnn.ipynb` | The same task with a convolutional network |
| `04a_asl_augmentation.ipynb` | Data augmentation to close the train/validation gap |
| `04b_asl_predictions.ipynb` | Deploying the trained model on new images |
| `05a_doggy_door.ipynb` | Transfer learning with a pretrained VGG16 (ImageNet) |
| `05b_presidential_doggy_door.ipynb` | Fine-tuning a pretrained model on a small custom dataset |
| `06_nlp.ipynb` | Introduction to NLP with a pretrained language model |

## PyTorch practice

| Notebook | Topic |
|---|---|
| `00_pytorch_fundamentals.ipynb` | Tensors, shapes, devices |
| `01_pytorch_workflow.ipynb` | Data → model → loss → optimiser → evaluation loop |
| `02_pytorch_classification.ipynb` | Binary and multi-class classification, non-linearity |
| `03_pytorch_computer_vision.ipynb` | FashionMNIST, CNNs, confusion matrix |
| `04_pytorch_custom_datasets.ipynb` | Custom `Dataset` / `DataLoader`, augmentation |
| `05_pytorch_going_modular.md` | Turning notebook code into reusable modules |
| `06_pytorch_transfer_learning.ipynb` | Transfer learning with `torchvision` models |
| `07_pytorch_experiment_tracking.ipynb` | Tracking experiments with TensorBoard |
| `08_pytorch_paper_replicating.ipynb` | Re-implementing a Vision Transformer from the paper |
| `09_pytorch_model_deployment.ipynb` | Model size / speed trade-offs and a demo app |

`utils.py` holds shared helpers; `model.pth` is a small trained checkpoint from the exercises.

## Running

```bash
git clone https://github.com/furkanselimozkan07/nvidia-deep-learning.git
cd nvidia-deep-learning
pip install torch torchvision matplotlib jupyterlab
jupyter lab
```

The DLI notebooks were written for NVIDIA's hosted GPU environment, so some dataset paths
need adjusting to run locally.

## Where this went next

I use these foundations in UAV perception work — real-time YOLO detection, geolocation and
payload delivery: [uav-perception-payload](https://github.com/furkanselimozkan07/uav-perception-payload).
