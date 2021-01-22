# Background (Terry v. Ohio):
In 1967 three men were stopped by a policeman described to be in plain clothes. This stop resulted in the officer frisking the men based on his belief that they were suspicious and led him to find weapons on two out of three of the men. It was argued that this stop violated the men’s Fourth Amendment right which protects people from unreasonable searches and seizure by the government. In an 8 to 1 decision it was deemed by the court that the officer did not violate the Fourth Amendment. 

# The problem:
In the fifty plus years since this case, people have been more concerned with police abuse of power and not having individual rights respected. Oftentimes, laws seem more black and white, or binary, but when a case is to be heard by a judge or jury emotions can get thrown into the mix for better or worse which can introduce bias. 

The goal of this analysis is to limit the amount of bias and have a machine classifier be the judge of whether these recorded stops infringed on a person’s Fourth Amendment right. With this information further analysis will be done to determine how big of a role race and gender plays in, as well as if there is an increase or decrease in occurrences based on time and day.

## Exploratory Data Analysis
When viewing values for if someone was frisked and if they were arrested, it was discoved that out of 44,859 stops there were 2,735 arrests made. However 10,104 people were frisked. This means that approximately 73% of people that were frisked were completely innocent and not arrested.

![alt text](https://github.com/melfriedman/FriskAnalysis/blob/main/images/Frisk%20graph.png?raw=true)

While it is assumed that someone having a weapon on them will effect this outcome, is this what the data will show? And if not is frisking someone even necessary for making an arrest if this affects innocent people?

![alt text](https://github.com/melfriedman/FriskAnalysis/blob/main/images/Feature%20Importance%20Plot.png?raw=true)
Besides being an unknown or unreported race, Black African Americans have the most influence on the preliminary model.

## Models used:
Logistic Regression

Decision Trees:
* Base Decision Tree model
* Bagged Trees
* Random Forests

XGBoost

## Final Model
While the final models had about 94% accuracy, there is still plenty of room for optimizing the parameters (for XGBoost). Going forward more adjustments on the parameters and possibly making adjustments to further clean up the data set to prevent overfitting could further improve the model.

#### Sources and More Information
Data from https://catalog.data.gov/dataset/terry-stops

Case info for Terry v. Ohio www.oyez.org/cases/1967/67

Fourth Amendment https://www.constituteproject.org/constitution/United_States_of_America_1992#145
