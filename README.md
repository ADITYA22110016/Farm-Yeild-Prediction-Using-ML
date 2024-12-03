# Farm-Yeild-Prediction-Using-ML


🌾 Dataset Overview
This dataset provides insights into various aspects of agriculture 🌱, specifically focusing on farm-level details, crop types, irrigation methods, soil properties, and associated metrics such as yield, water usage, fertilizer usage, and pesticide usage. The goal is to analyze and predict crop yields and identify factors that influence productivity.

🔑 Key Features:
🏷️ Farm_ID: Unique identifier for each farm.
🌽 Crop_Type: Type of crop cultivated (e.g., Cotton, Carrot, Wheat).
🚿 Irrigation_Type: Method of irrigation used (e.g., Drip, Manual, Flood).
🌍 Soil_Type: Type of soil present on the farm (e.g., Loamy, Sandy, Silty).
🗓️ Season: The season in which the crop is grown (e.g., Kharif, Rabi, Zaid).
🏞️ Farm_Area (acres): Total area of the farm in acres.
🧪 Fertilizer_Used (tons): Quantity of fertilizer applied.
🐞 Pesticide_Used (kg): Amount of pesticide used.
💧 Water_Usage (cubic meters): Total water usage for the crop.
📈 Yield (tons): Total yield of the crop in tons.
🎯 Objective:
The primary objective is to analyze the relationships between these variables, identify factors that influence crop yields, and build predictive models to estimate yields based on input features.

📊 Data Characteristics:
📝 Data Type: The dataset contains both numerical and categorical features.
🎯 Target Variable: Yield(tons)
🔢 Encoded Features: Categorical variables such as Crop_Type, Irrigation_Type, and Soil_Type are encoded for modeling purposes.
🤖 Modeling Approach:
Regression Models Used:
🧮 Linear Regression
🌲 Random Forest Regressor
⚡ XGBoost Regressor
💡 LGBM Regressor


Key Observations:
Correlation with Yield(tons):

Farm_Area(acres): There is a positive correlation with yield (0.15). Larger farm areas tend to show a slight increase in yield, indicating that farm size might contribute to productivity, but the relationship is weak.
Fertilizer_Used(tons): The correlation is positive but weak (0.045). This suggests that while fertilizer contributes to yield improvement, it is not a dominant factor on its own.
Water_Usage(cubic meters): There is a positive correlation (0.11), indicating that higher water usage is generally associated with higher yields, as water availability is crucial for crop productivity.
Crop Types: Some specific crop types like Crop_Type_Carrot (0.21) and Crop_Type_Tomato (0.18) exhibit positive correlations with yield, indicating that these crops may have higher yield potential.
Relationship Among Inputs:

Fertilizer_Used(tons) and Pesticide_Used(kg): There is a very weak negative correlation (-0.045). This suggests that the two inputs are not directly correlated, and their application may vary based on crop-specific needs.
Fertilizer_Used(tons) and Water_Usage(cubic meters): A positive correlation (0.012) indicates that more fertilizer might coincide with more water usage, though the relationship is not strong. Effective fertilization often requires adequate water to maximize nutrient uptake.
Farm_Area(acres):

Farm_Area(acres) and Water_Usage(cubic meters): A weak negative correlation (-0.04) suggests that larger farms do not necessarily use more water per acre, reflecting possible variations in irrigation practices.
Farm_Area(acres) and Fertilizer_Used(tons): A weak negative correlation (-0.13) shows that larger farms might use slightly less fertilizer per acre, perhaps reflecting efficiency measures or more extensive cultivation practices.
Impact of Soil Type and Season:

Soil_Type_Loamy: Positively correlated with Yield(tons) (0.02), indicating that loamy soil is generally favorable for higher yields due to its balanced moisture and nutrient retention capabilities.
Season_Kharif and Yield(tons): A positive correlation indicates that Kharif season crops generally have higher yields, possibly due to favorable weather and water availability.
Irrigation_Type Effects:

Irrigation_Type_Manual and Yield(tons): Shows a moderate positive correlation (0.19), suggesting that manually irrigated farms may focus on crops with higher yields or have more tailored irrigation practices.
Irrigation_Type_Flood and Yield(tons): Negative correlation (-0.27) suggests that flood irrigation may not always lead to the highest yields and could relate to inefficiencies or waterlogging.
Crop-Specific Observations:

Crop_Type_Cotton has a negative correlation with Yield(tons) (-0.19), reflecting its potentially lower average yield compared to other crops.
Crop_Type_Potato has a positive correlation with Fertilizer_Used(tons) (0.34), suggesting higher input requirements.
Summary Insights:
Farm Size Influence: While larger farm areas have a weak positive correlation with yield, resource inputs do not scale linearly with size, indicating diverse management practices.
Resource Optimization: Fertilizer, water, and pesticide inputs have varying degrees of correlation with yield, emphasizing the need for crop-specific management strategies.
Soil and Season Importance: Loamy soil and Kharif season tend to positively influence yields, while irrigation type and specific crop types have varying impacts.
