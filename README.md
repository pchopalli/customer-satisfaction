##                                               Customer Satisfaction Prediction Model
![customer-experience](https://github.com/pchopalli/customer-satisfaction/assets/85187674/db645871-e5e8-4095-9ea9-84015e46795b)

As a logistic provider, the company wants to learn if it's customers are happy The expansion strategy depends on the information if the customers are happy and the only way to do that is to measure how happy each customer is. If we can predict what makes our customers happy or unhappy, we can then take necessary actions.

The constant feedback provided by customers to be used to develop a prediction model for customer satisfaction

Various models were trained and validated in our approach to find the best model to solve our problem. Logistic Regression model with default parameters and then the hyperparameters were tuned, this model didn't give the best accuracy. SVM model was trained with default values, polynomial and hyperparamter tuning. SVM model with polynomial=3 gave better accuracy but it was not the best accuracy. RandomForest model was trained with default and hyperparamter tuning and the accuracy was low. VotingClassifer and AdaBoost models were also trained with accuracy not any better than other models

Feature Engineering was used to select the best features. After dropping less simportant features , the model was trained using Random Forest which resulted in accuracy of 85%. Since the data set was very small it was effective to use only the best features to address the below. Below table shows all the models used for training and the associated accuracies

<table>
        <tr>,
            <th> Model </th>
            <th> Training Accuracy </th>
            <th> Test Accuracy </th>
        </tr>
            <tr>
            <th> SVM </th>
            <th> 0.78 </th>
            <th>0.62 </th>
        </tr>
            <tr>
            <th> SVM(Polynomial) </th>
            <th> 0.8 </th>
            <th> 0.73 </th>
        </tr>
            <tr>
            <th> Logistic Regression </th>
            <th> 0.57 </th>
            <th> 0.62 </th>
        </tr>
            <tr>
            <th> Random Forest </th>
            <th> 0.96 </th>
            <th> 0.61 </th>
        </tr>
            <tr>
            <th> Random Forest(Hyperparameter Tuning) </th>
            <th> 0.57 </th>
            <th> 0.62 </th>
        </tr>
           <tr>
            <th> Random Forest(Feature Engineering) </th>
            <th> 0.82 </th>
            <th> 0.85 </th>
        </tr>
        <tr>
            <th> Voting Classifier </th>
            <th> 0.87 </th>
            <th> 0.69 </th>
        </tr>
         <tr>
            <th> AdaBoost</th>
            <th> 0.96 </th>
            <th> 0.61 </th>
        </tr>
        </table> 
        
The model developed provides us with the resource to predict and understand the satification of our customers. This will help us take any required corrective action towards likely unhappy customers to retain business. Upon receiving the survey based on model predictions we can see the breakdown of happy and unhappy customers and take any required actions
