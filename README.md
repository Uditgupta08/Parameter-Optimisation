# SVM Optimization on UCI Dataset

## 📊 Project Overview
This project performs Support Vector Machine (SVM) optimization on a multi-class dataset from the UCI Machine Learning Repository. It includes 10 randomized train-test splits, hyperparameter optimization using randomized search (100 iterations per split), convergence analysis, and basic data analytics. The project is implemented using Python and popular machine learning libraries.

## 📁 Dataset Used
- **Dataset**: Occupancy Estimation (UCI Repository)
- **Link**: [UCI Repository - Occupancy Estimation](https://archive.ics.uci.edu/ml/datasets/Occupancy+Detection+)
- **Rows**: ~10,129
- **Target Column**: `Room_Occupancy_Count`

> Note: Although the dataset used is binary, it may be replaced with a multi-class dataset such as Letter Recognition if required.

## 🛠️ Technologies & Libraries
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

## 🔄 Methodology
1. **Dataset Selection**: Chosen from UCI with rows between 5k and 30k.
2. **Preprocessing**: Dropped time columns, handled missing values, scaled features.
3. **Train-Test Split**: Dataset split into 70-30 ratio, repeated 10 times with different random states.
4. **Hyperparameter Optimization**:
   - Kernels: `linear`, `rbf`, `sigmoid`, `poly`
   - Parameters: `C`, `gamma`
   - Optimized using randomized values for 100 iterations per split.
5. **Best Parameters Table**: Accuracy and hyperparameters stored for each split.
6. **Convergence Plot**: Learning curve plotted for the best-performing split.
7. **Basic Analytics**: Target count plot, feature description, null value check, and correlation analysis.

## 📈 Results
- Reported accuracy and best parameters for each of the 10 samples.
- Highest accuracy sample visualized using a convergence (learning) curve.

