# NYC-Taxi-ML-model

## Build machine learning model

### Overview 
To build a machine learning model to predict whether a NYC TLC taxi cab rider will be a generous tipper.

### Problem 
After rejecting the initial modeling objective (predicting non-tippers) out of ethical concern, it was decided to predict “generous” tippers—those who tip ≥ 20%. This decision was made to balance the sometimes competing interests of taxi drivers and potential passengers.

### Solution 
I used two different modeling architectures and compared their results. Both models performed acceptably, with a random forest architecture yielding slightly better predictions. As a result, I would recommend beta testing with taxi drivers to gain further feedback. 

## Methodologies
### PACE framework
1. Plan
   - The ethical implications of the model, the consequences of the model making errors.
   - Target variable
   - Features need to make this prediction
2. Analyze
   - Feature engineering
3. Construct
   - Modeling
4. Excecute
   - Conclusion
   - Data interpretation

### Detail
The assumption was that a trip’s itinerary, predicted fare amount, and time of day may have a strong enough relationship with tip amount that we could accurately predict generous tipping. After I built the identified models and performed the testing, it is clear that these factors do indeed help predict tipping. The model’s F1 score was 0.7451.

### Summary
The resulting algorithm is usable to predict riders who might be generous tippers, with reasonably strong precision, recall, F1, and overall accuracy scores. Refer to the “next steps” section for suggestions.

#### Future model suggestions
- Collect/add more granular driver and user-level data, including past tipping behavior.
- Cluster with K-means and analyze the clusters to derive insights from the data
