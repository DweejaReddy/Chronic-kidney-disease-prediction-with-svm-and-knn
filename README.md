# Chronic kidney Disease prediction using KNN and SVM
1. First loading of the dataset (kidney_disease.csv) using pandas.
2. Dropping unwanted columns in the dataset.
3. Renaming the columns to make it more user-friendly.
 ['age', 'blood_pressure', 'specific_gravity', 'albumin', 'sugar', 'red_blood_cells', 'pus_cell’  'pus_cell_clumps', 'bacteria', 'blood_glucose_random', 'blood_urea', 'serum_creatinine', 'sodium', 'potassium', 'haemoglobin', 'packed_cell_volume', 'white_blood_cell_count', 'red_blood_cell_count',
 'hypertension', 'diabetes_mellitus', 'coronary_artery_disease', 'appetite', 'peda_edema' 'aanemia', 'class']
4. Detecting columns that are required to convert into numerical datatype and converting them into numerical datatype.
5. Extracting categorical and numerical columns from the dataset.
6. Finding unique values in categorical columns.
* red_blood_cells has [nan 'normal' 'abnormal'] values
* pus_cell has ['normal' 'abnormal' nan] values
* pus_cell_clumps has ['notpresent' 'present' nan] values
* bacteria has ['notpresent' 'present' nan] values
* hypertension has ['yes' 'no' nan] values
* diabetes_mellitus has ['yes' 'no' ' yes' '\tno' '\tyes' nan] values
* coronary_artery_disease has ['no' 'yes' '\tno' nan] values
* appetite has ['good' 'poor' nan] values
* peda_edema has ['no' 'yes' nan] values
* aanemia has ['no' 'yes' nan] values
* class has ['ckd' 'ckd\t' 'notckd'] values
7. Replace incorrect values of the columns from the dataset.
8. Check for null values in the columns.
9. Now fill the null values by using two methods 
* Random sampling for higher null values
* mean/mode sampling for lower null values
10. Now splitting of dataset into training set and testing set.
11. Now import KNeighborsClassifier and Linear SVM classifier from sklearn.neighbors and sklearn.svm respectively.
