# An-Intelligent-Decision-Support-System-for-Financial-Institution.

Introduction:

Food insecurity is a critical global challenge affecting millions of people worldwide and particularly in developing countries. This menace of food insecurity is attributed to the
changing climatic conditions which in turn impede crop production. The changes in weather patterns are so severe and unpredictable that potential investors are hesitant to fund large-scale agricultural schemes for fear of poor yields. These complexities have ultimately created an undesirable situation whereby large-scale schemes are underfunded while smallscale farmers are completely unable to sustain their subsistence crops. Eventually, the global economy has become exposed to acute shortages in crop production leading to increasing incidences of food crisis across the world. Therefore, there is an urgent need for scientific investigation into the possible intelligent decision support systems that can be embraced to improve crop production and quell the impending widespread crisis.

![image](https://github.com/user-attachments/assets/9cc705d3-66e7-4f37-b2d0-81af9115c731)




# Model
---

The decision tree model was used in training and testing the intelligent decision support system. It comprised of a hierarchical structure that accomplishes predictions or classifications through recursive partitioning of a dataset based on the given input features. The dataset used in this project was downloaded from
dataverse.harvard.edu. The dataset had 8 features, with 7 of them being input features and the remaining 1 being the output
feature. Out of the 7 input features, 4 of them namely ‘Nitrogen’, ‘Phosphorous’, ‘Potassium’, and ‘pH’ denoted soil conditions while the other 3 namely ‘temperature’, ‘humidity’, and ‘rainfall’ represented climatic conditions. The output feature called ‘label’ was the representation of the different types of crops.

Python’s pandas library was used for pre-processing the dataset, matplotlib was also applied for visualization, and sklearn was used for building the decision tree. Useful modules from the sklearn library like DecisionTreeClassifier, train_test_split, and accuracy_score were then applied in facilitating and validating the model.
The decision tree modelling process started from the splitting criteria whereby the dataset was divided into subsets at each node of the tree. The splitting process was facilitated by two criteria called Gini impurity and entropy. The Gini Impurity (I_Gini) measured the level of disorder or impurity in the given dataset. For every node with multiple classes, like ‘Nitrogen’ or ‘Potassium’ or ‘Rainfall’, the Gini impurity would get calculated as follows:
I_Gini=1 - ∑_(i=1)^n▒〖p_i〗^2 
where: I_Gini = Gini impurity

# Results
---
A.	Data Overview
The dataset contained 8 columns which basically represent the crop types, soil, and weather conditions. The specific column names include; Nitrogen, Phosphorous, Potassium, and pH which portray the soil conditions; temperature, humidity, and rainfall depicting the weather conditions; and label which represent the corresponding crop type. The total number of records in the dataset is 2,200. Snippet of the table is shown below.

<img width="1245" alt="Screenshot 2025-07-01 at 09 01 45" src="https://github.com/user-attachments/assets/771a94a4-1a40-4e35-a4a2-77081981e1de" />

B.	Average Temperature for Each Crop Type
Fig.1 gives insights pertaining to the optimum temperature conditions for each type of crop. The results can be used in postulating that areas experiencing high temperatures due to climate change should shift to planting Papayas, Mangoes, and Blackgram.

<img width="235" alt="image" src="https://github.com/user-attachments/assets/27978888-209b-434c-9590-b9722da0d8b2" />

C.	Average Rainfall for Each Crop Type
Fig.2 shows the optimum rainfall conditions for different crop types. It can be deduced that extreme changes in climate like heavy rainfall or extended drought should not pose any threat to crop production. Rather, both small-scale and large-scale farmers should dynamically shift to cultivating the right type of crops; rice during very heavy rains; maize, banana, and apples during moderate rains; muskmelon and lentil during extended drought.

<img width="249" alt="image" src="https://github.com/user-attachments/assets/0d32494a-0f50-4666-981e-f0e8e06caa83" />

D.	Optimum Soil Nutrient Composition for Each Crop Type
Fig.3 shows the optimum composition of soil nutrients that support the yields of different crop types. Apple requires very high amounts of potassium and phosphorus more than any other crop. Banana, coffee, cotton, rice, and watermelon require a lot of nitrogen more than they require phosphorous or potassium. Such insights are very useful in providing the right conditions for achieving increased crop production despite the threats of climate change.

<img width="251" alt="image" src="https://github.com/user-attachments/assets/12c74317-21ec-400c-8681-1fafcc18c227" />

E.	Decision Tree Model
The confusion matrix of the decision tree model developed in this project. The accuracy of the model in predicting suitable crops for an area was determined to be 98% thereby justifying an overwhelming performance in intelligent decision making. The correct predictions along the diagonal are clearly way higher than the false positives and false negatives found off the diagonal.

<img width="248" alt="image" src="https://github.com/user-attachments/assets/d5b88fd5-cfc6-416b-b39e-5733cdb4fb9c" />

#Conclusion

The idea was conceptualised to demonstrate how financial institutions can use data modelling techniques to make informed decisions in supporting agriculture and enhancing food security. The results indicated a 98% accuracy score to affirm that decision tree model is a reliable method for predicting crop production patterns. The novelty of the current research is that it developed a generalisable and scalable decision tree model that is not restricted to any geographical area. The model is highly adaptable 
and usable in all regions of the world where the investors intend to support agricultural initiatives. As a result, the current research will enable food security in Africa and other regions of the world since investors will manage to identify the most suitable crops that can withstand the prevailing climatic conditions. For instance, an area could be initially suitable for maize cultivation but then the area becomes no longer suitable for the crop due to harsh changes in climate. Instead of the residents languishing in hunger due to the poor harvests of maize, the investors can simply use the model to predict the new crop type that can withstand such changes and then provide the necessary support in cultivating the new crop like mangoes, cassava, wheat, or banana.









