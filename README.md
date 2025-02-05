# Water Potability Prediction

## Introduction
The goal of this project is to perform exploratory data analysis (EDA), prepare the data for modeling, train and evaluate the data through various machine learning models, and present the results.<br>
The dataset chosen is from Kaggle, which predicts water potability using various water quality attributes.<br>
Original Dataset Source: [Kadiwal, Aditya. (2020). Water Quality. Kaggle.](https://www.kaggle.com/datasets/adityakadiwal/water-potability)

## Water Quality Dataset Description
The dataset for this project focuses on predicting the potability of water, where potability is represented as a categorical variable with values of 0 or 1. The primary goal is to develop a dependable prediction model based on nine numerical features. Each feature is of type float, indicating a numeric nature, and contributes distinct information to the analysis. Notably, the features exhibit variations in scale, reflecting their diverse measurement units.

### Attributes of Dataset:
1. _pH value:_ PH is an important parameter in evaluating the acid–base balance of water. It is also the indicator of acidic or alkaline condition of water status. WHO has recommended maximum permissible limit of pH from 6.5 to 8.5. The current investigation ranges were 6.52–6.83 which are in the range of WHO standards.
2. _Hardness:_ Hardness is mainly caused by calcium and magnesium salts. These salts are dissolved from geologic deposits through which water travels. The length of time water is in contact with hardness producing material helps determine how much hardness there is in raw water. Hardness was originally defined as the capacity of water to precipitate soap caused by Calcium and Magnesium.
3. _Solids (Total dissolved solids - TDS):_ Water can dissolve a wide range of inorganic and some organic minerals or salts such as potassium, calcium, sodium, bicarbonates, chlorides, magnesium, sulfates etc. These minerals produced un-wanted taste and diluted color in appearance of water. This is the important parameter for the use of water. The water with high TDS value indicates that water is highly mineralized. Desirable limit for TDS is 500 mg/l and maximum limit is 1000 mg/l which prescribed for drinking purpose.
4. _Chloramines:_ Chlorine and chloramine are the major disinfectants used in public water systems. Chloramines are most commonly formed when ammonia is added to chlorine to treat drinking water. Chlorine levels up to 4 milligrams per liter (mg/L or 4 parts per million (ppm)) are considered safe in drinking water.
5. _Sulfate:_ Sulfates are naturally occurring substances that are found in minerals, soil, and rocks. They are present in ambient air, groundwater, plants, and food. The principal commercial use of sulfate is in the chemical industry. Sulfate concentration in seawater is about 2,700 milligrams per liter (mg/L). It ranges from 3 to 30 mg/L in most freshwater supplies, although much higher concentrations (1000 mg/L) are found in some geographic locations.
6. _Conductivity:_ Pure water is not a good conductor of electric current rather’s a good insulator. Increase in ions concentration enhances the electrical conductivity of water. Generally, the amount of dissolved solids in water determines the electrical conductivity. Electrical conductivity (EC) actually measures the ionic process of a solution that enables it to transmit current. According to WHO standards, EC value should not exceeded 400 μS/cm.
7. _Organic_carbon:_ Total Organic Carbon (TOC) in source waters comes from decaying natural organic matter (NOM) as well as synthetic sources. TOC is a measure of the total amount of carbon in organic compounds in pure water. According to US EPA < 2 mg/L as TOC in treated / drinking water, and < 4 mg/Lit in source water which is use for treatment.
8. _Trihalomethanes (THMs):_ THMs are chemicals that may be found in water treated with chlorine. The concentration of THMs in drinking water varies according to the level of organic material in the water, the amount of chlorine required to treat the water, and the temperature of the water that is being treated. THM levels up to 80 ppm is considered safe in drinking water.
9. _Turbidity:_ The turbidity of water depends on the quantity of solid matter present in the suspended state. It is a measure of light emitting properties of water and the test is used to indicate the quality of waste discharge with respect to colloidal matter. The mean turbidity value obtained for Wondo Genet Campus (0.98 NTU) is lower than the WHO recommended value of 5.00 NTU.
10. _Potability:_ Indicates if water is safe for human consumption where 1 means Potable and 0 means Not potable.

### Missing values:
- ph: 491
- Sulfate: 781
- Trihalomethanes: 162

### Duplicated values:
There are no duplicate values in the dataset.

## Framing the Problem and Looking at the Big Picture
### Frame the Problem
1. Supervised learning – training examples are labeled.
2. A classification task – predict a category.
3. Batch learning
    - Small data set
    - No continuous flow of data coming into the system
    - No need to adjust to changing data rapidly

The objective is to find a model that allows us to predict whether the water in a river is drinkable or not to know if we should invest in the development of a sanitation network of water. This task will therefore be binary classification, we will assign in the remainder of this project the value 1 for “Drinkable” and 0 for “Non-Drinkable”.

### Look at the big picture
Predictions will be used to help inform people if the body of water is drinkable. This will be done through the following properties of the water: pH value, hardness, solids, chloramines, sulfate, conductivity, organic carbon, trihalomethanes, and turbidity.

<hr>

Please view the [notebook](https://github.com/Verma-Aakanksha/EECS3401-Project/blob/master/EECS-3401-Project.ipynb "Water Potability Prediction Notebook") for the code, equations, visualizations, and other computational outputs for the project.<br>
Please view the [report](https://github.com/Verma-Aakanksha/EECS3401-Project/blob/master/EECS%203401%20-%20Project_Water%20Potability%20Prediction.pdf
 "Water Potability Prediction Report") for more detailed information about this project.
