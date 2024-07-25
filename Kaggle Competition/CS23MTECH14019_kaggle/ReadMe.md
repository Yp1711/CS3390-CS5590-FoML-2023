## Kaggle Hackathon 2023

### **Folder Contains**
* Gradient Boosting - 57.024% (Public) & 44.352% (Private)
    * Gradient Boosting.ipynb
    * predictions_gradient_boosting.csv
* Weighted Mode - 63.227% (Public) 48.169% (Private)
    * Weighted Mode.ipynb
    * predictions_weighted_mode.csv    

### **To run the Gradient Boosting Model**
```bash
- Run Gradient Boosting i.e.[GradientBoostingClassifier()] with Hyperspecific parameters, whose instance is stored in model_GB

- The Prediction on the testing datset is stored as "predictions_gradient_boosting.csv"
```
### **To run the Weighted Mode Model**
```bash
- Run Random Forest i.e[RandomForestClassifier()] with specific Hyperparameters, whose instance is stored in model_1

- Run Decision Tree i.e[DecisionTreeClassifier()] with specific Hyperparameters, whose instance is stored in model_2 

- Run KNN i.e[KNeighborsClassifier()] with specific Hyperparameters, whose instance is stored in model_3 

- The Weighted Prediction on the testing datset is stored as "predictions_weighted_mode.csv"

```

### **Accuracy Score**
* **Weighted Mode**
```bash
48.169% (Private)
63.227% (Public)
```
* **Gradient Boosting**
```bash
44.352% (Private)
57.024% (Public)
```