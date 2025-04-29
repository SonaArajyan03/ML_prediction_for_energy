# ML_prediction_for_energy
A machine learning model using Random Forest to predict energy minimization in an elastic rod under vibration. The project includes preprocessing of mechanical data, feature selection, and model evaluation using confusion matrix and classification report.


⚙️ Energy Optimization using Random Forest
This project demonstrates the use of a Random Forest Classifier to predict whether a physical system is in a state of minimized total energy. The model is trained on pre-processed data representing the stress-strain state of an elastic rod subjected to longitudinal vibrations.

🧠 Model Goal
The main goal is to classify system states as either "Minimized" or "Not Minimized" in terms of total energy, based on mechanical and physical input features.

📊 Dataset and Features
Input features include various mechanical properties and derived quantities related to vibration and deformation.

The target variable is Minimized, derived from a threshold on the Total_Energy column.

🔍 Preprocessing
Categorical and interval-type data are encoded using one-hot encoding or transformed to numerical values.

Special care is taken to handle pandas.Interval types that arise from binning operations (e.g., pd.cut()), converting them into midpoints or dummies for compatibility with scikit-learn.

🚀 Model
Algorithm: RandomForestClassifier from scikit-learn

Evaluation: Confusion matrix and classification report are used to assess model performance.

📦 Dependencies
pandas

scikit-learn

numpy
