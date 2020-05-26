# Hierarchical Clustering on Cereal Data
The clustering technique can be very handy when it comes to unlabeled data. Since most of the data in the real-world is unlabeled and annotating the data has higher costs, clustering techniques can be used to label unlabeled data.

## 1. Project Definition
**Purpose**:
The purpose of this project is to find several groups of most suitable cereals from the dataset and the 
correlation between each of the ingredients to have better knowledge so that it is to possible suggest 
a specific kind of cereals to a exact group of consumers/customers/patients.

**Project Scope**: After having the cut-point on the dendogram to find several clusters for a broad 
knowledge discovery.

**Key Stakeholders**: The key stake holders are all individuals who consume cereal on regular basis for 
breakfast or dinner or even as a snack.

## 2. Literature Survey
There have been no comprehensive reviews of the relation of breakfast cereal consumption to nutrition 
and health. Breakfast cereal consumption is associated with diets higher in vitamins and minerals and 
lower in fat but is not associated with increased intakes of total energy or sodium or risk of dental caries. 
Most studies on the nutritional impact are cross-sectional, with very few intervention studies, so 
breakfast cereal consumption may be a marker of an overall healthy lifestyle. Breakfast cereals have 
become immensely popular in fast-moving countries, as they provide a bowl full of nutrients in a short 
and simple way.

So, this report may help to those who want a healthy breakfast by given them proper data analysis.

## 3. Dataset Description

**Data source:** [Healthy Breakfast Story](https://dasl.datadescription.com//Stories/HealthyBreakfast.html) at StatLab ( http://lib.stat.cmu.edu/ ) 

**Data files:** 
1. [cereal.txt](https://www.cs.umd.edu/hcil/hce/examples/cereal/cereal.txt) (without 'vitamin' and 'rating' columns) : 77 x 9
2. [cereal-updated.txt](https://www.cs.umd.edu/hcil/hce/examples/cereal/cereal-updated.txt) (with 'vitamin' and 'rating' columns) : 77 x 11

**The meaning of each column :**
1. 1st column: Name of cereal
2. **calories**: calories per serving
3. **protein**: grams of protein
3. **fat**: grams of fat
4. **sodium**: milligrams of sodium
5. **fiber**: grams of dietary fiber
6. **carbo**: grams of complex carbohydrates
7. **sugars**: grams of sugars
8. **potass**: milligrams of potassium
9. **vitamins**: vitamins and minerals - 0, 25, or 100, indicating the typical percentage of FDA recommended
10. **shelf**: display shelf (1, 2, or 3, counting from the floor)
11. **rating**: a rating of the cereals (calculated by Consumer Reports)

## 4. Methodology
**Step 1:** At first, import the dataset into .csv format from .txt file.

**Step 2:** Import necessary libraries

**Step 3:** Read the dataset and store it into pandas dataframe

**Step 4:** Then, data Preparation is done. Missing values are filled up by the mean values of those attributes respectively.

**Step 5:** Find the number of clusters from Dendrogram

**Step 6:** Fitting Hierarchical Clustering to the Cereals and predict

**Step 7:** Finally, clusters are seperated.

## 5. Questions
Use the given data files to find the following: 
1. Is a strong correlation between dietary fiber and potassium?  
2. See other correlation between the data given in the files.
3. Try to find some other information
4. Are groups of cereals from which we can choose according to our preferences?


## References
### Finding Correlation Between Many Variables in Python
1. [pandas.DataFrame.corr](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.corr.html)
2. [Pearson Coefficient of Correlation with Python](https://levelup.gitconnected.com/pearson-coefficient-of-correlation-using-pandas-ca68ce678c04)
3. [seaborn.heatmap](https://seaborn.pydata.org/generated/seaborn.heatmap.html)
