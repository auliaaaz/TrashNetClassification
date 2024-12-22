# TrashNetClassification
This project focuses on classifying waste images into six categories: Cardboard, Glass, Metal, Paper, Plastic, and Trash. The model was trained using PyTorch and fine-tuned for optimal performance. The repository includes the Jupyter Notebook used for training, as well as the necessary files to reproduce the results.

**Performance Metrics:**
| Category   | Precision | Recall | F1-Score | Support |
|------------|-----------|--------|----------|---------|
| Cardboard  | 0.99      | 0.95   | 0.97     | 161     |
| Glass      | 0.92      | 0.98   | 0.95     | 200     |
| Metal      | 0.97      | 0.93   | 0.95     | 164     |
| Paper      | 0.97      | 0.96   | 0.96     | 238     |
| Plastic    | 0.96      | 0.95   | 0.96     | 193     |
| Trash      | 0.90      | 0.96   | 0.93     | 55      |

## Installation
To set up the project, follow these steps:
1. Clone the repository:
   ```bash
   git clone https://github.com/https://github.com/auliaaaz/TrashNetClassification.git
   cd TrashNetClassification
2. Install the dependencies:
    ```bash
    pip install -r requirements.txt
3. Set up the environment variable for W&B, you can use GitHub secrets if using GitHub Actions.
    ```bash
    WANDB_API_KEY=<your-wandb-api-key>

### To Train or Use the Model
1. Run the Notebook:
Open TrashNetClassification.ipynb in Jupyter Notebook or any compatible platform to train or evaluate the model.

2. Use the Pretrained Model:
Directly use the provided ```best_model.pth``` for testing or fine-tuning.
Model download URL: https://github.com/auliaaaz/TrashNetClassification/actions/runs/12453547135/artifacts/2353378179

3. Automated Workflow:
The workflow file ```.github/workflows/run-notebook.yml``` automates the training and evaluation process. Simply trigger the workflow manually or on code pushes to reproduce results.

