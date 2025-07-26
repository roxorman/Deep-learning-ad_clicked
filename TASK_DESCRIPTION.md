# Ad Click Prediction from Cursor Movement Images

## Task Description

The objective is to predict whether a user clicked on an advertisement based on images of their cursor movements. The dataset is sourced from [The Attentive Cursor Dataset](https://gitlab.com/iarapakis/the-attentive-cursor-dataset).

### Data Sources
- **Image Data**: A zip file containing `.png` images of cursor movements, available at [Google Drive](https://drive.google.com/file/d/18c43SiRTrJYjUN0cPoynA39NWx__bJDa/view?usp=drive_link).
- **Target Data**: A dataset with the target variable, available at [Google Drive](https://drive.google.com/file/d/1_lwltpA4uhAchTHy7M6fe3tM_eCRGqjU/view?usp=drive_link).
  - **Target Variable**: `ad_clicked` column.
  - **Image Identifier**: `log_id`, corresponding to the filename of each `.png` image.

## Task Requirements

1. **Download the Data**:
   - Retrieve the image and target data from the provided links.
2. **Create Labels**:
   - Map the `ad_clicked` column to the corresponding image files using `log_id`.
3. **Display Images**:
   - Visualize a few sample images to understand the cursor movement patterns.
4. **Split Data**:
   - Divide the dataset into training, validation, and test sets.
5. **Model Development**:
   - Develop a neural network (NN) model to predict ad clicks.
   - Tune hyperparameters and monitor convergence behavior to achieve the highest possible accuracy on the test set.
6. **Model Saving**:
   - Save the model with the best performance (highest test accuracy) for future use, ensuring it is not just a one-time printout during training.
7. **Reflection**:
   - Critically evaluate the approach, including comparisons with alternative methods.
   - Document the reflection in a markdown cell.

## Objective
- Maximize model performance, specifically the accuracy on the test set, while ensuring generalization to unseen data.
- No specific accuracy target is provided, but the model should demonstrate robust performance on appropriate metrics.

## Constraints
- The best-performing model must be saved explicitly (e.g., using a model checkpointing mechanism) to allow reuse.
