### Find subpackage
This subpackage includes two modules named `Deficiency.py` and `Recommend.py`. This subpackage mainly aims at finding the deficient nutrient in a person and recommending corresponsing cereal(s) for them. 

**Deficiency.py**
This module includes a parent class 'Diet' and has the following:

* The module has three methods, one for initialising the name of the person, and second for setting the default values which has a dictionary with default gender-based nutrient values. It also has a display values method whcih will then be subsequently called during the execution of child class.

* Child class is called 'Deficieny' which consist of basic initialisation method along with three methods- women, men, and couple. The class takes women's cureent levels of nutrient values as input arguments, and their corresponding deficiency can be returned by calling the 'women' function. For determining the deficincy in men, we need to call 'men' function. Similarly for testing nutrient deficiency in a couple, need to call the 'couple' function. 

* Summing up, this module shows how a graphical representation of how much a person is short on essential nutrients specifically protein and calories.

**Recommend.py**
This module has two functions:
* recommend: Takes in the deficient protein amount and excess calories amount from the previous module (Deficiency.py), and gives a recommended cereals to compensate for the same. 

* mycereal: This function provides graphical representation of nutrient content and also the rating for the selected cereals. 

### MANUAL SUBPACKAGE:
This subpackage inculdes two modules named: `Person.py` and `Cereals.py`.  This package mainly aims at providing visualization of nutrient composition in each cereal and top countries for each type of deficiency.

**Cereals.py**
This modules has two methods: Display function for the nutrient composition in cereals and one a representation in world map for nutrient deficient countries.

* This method can be called when we want to see and understand the distribution of each nutrient in each type of cereal(here we have considered a dataset with 74 most popular brands in US). This function reads and displays the raw data available in an excel file in a pictorical format using pygal.

* This method gives us an idea about the most common nutrient deficiency in accordance to a person's place of origin. This data is obtained from authentic sources and simialr to WHO findings. (This is not meant show any racial bias)

**Person.py**
This module shows a default nutrient values for man and women(here we have restricted to the nutrients associated with cereals only). The module takes man and women as inputs and shows a default healthy man's required nutrient conmtents.





