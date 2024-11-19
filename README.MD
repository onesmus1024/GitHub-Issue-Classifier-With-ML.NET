# Categorizing Support Issues with Multiclass Classification Using ML.NET

This repository showcases a machine learning solution developed with ML.NET to classify GitHub issues based on their titles and descriptions.

## Key Features

- **Data Preparation**: Converts categorical labels into numeric keys, processes text fields into feature vectors, and combines them into a unified feature column.
- **Model Training**: Employs the SDCA Maximum Entropy trainer for efficient multiclass classification.
- **Evaluation**: Measures model performance using metrics like accuracy, log-loss, and log-loss reduction.
- **Prediction**: Enables real-time predictions for individual data points using the trained model.
- **Model Persistence**: Facilitates saving and reloading the trained model for deployment and reuse.

## Technology Stack

- **ML.NET**: Framework for building and training machine learning models.
- **C#**: Programming language used for implementing the pipeline and application logic.
- **.NET Core**: Ensures cross-platform compatibility.

## How It Works

1. **Data Preparation**:  
   - Reads input data from TSV files containing GitHub issue details.  
   - Fields include `Title`, `Description`, and `Area` (the classification label).  
   - Text fields are transformed into numeric representations, labels are encoded, and all features are combined into a `Features` column.

2. **Model Training**:  
   - The training pipeline processes the data and builds the model.  
   - The trained model is saved as a `.zip` file for future use.

3. **Evaluation**:  
   - A test dataset evaluates the model, providing metrics such as accuracy and log-loss.  

4. **Prediction**:  
   - The trained model can classify new GitHub issues based on their `Title` and `Description`.

## Prerequisites

- .NET Core SDK (version 3.1 or later)  
- Visual Studio or any C# IDE  
- ML.NET (version 1.5 or later)  

## Microsoft Documentation

This project is inspired by a tutorial from Microsoft Documentation.  
[Visit the tutorial here](https://learn.microsoft.com/en-us/dotnet/machine-learning/tutorials/github-issue-classification).

## Use Cases

- Categorizing GitHub issues for better management.
- Adapting the solution to classify support tickets, emails, or other text-based data.
- Exploring ML.NET's multiclass classification capabilities.
