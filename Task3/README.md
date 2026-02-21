Each group member should provide feedback on the other group members’ work. Be detailed and specific where possible. The quality of this feedback can play a part in your grade.

You can provide feedback to your group members in many different ways (live in a meeting, offline, or however else you devise) but the feedback must be documented here! 

Please replace “Feedback giver #x” with a group member’s name below and add feedback as a bulleted list below. Note: There is a pencil icon on the top right of the README file (when you are viewing the README.md file) that allows you to edit.

- Bing
  + I think it'd be helpful to write out the equation for both model.
  + Give a short narrative on what each function is doing, how does it do what it do.
  + Write out the final model equation and interpret the coefficients. 
  + Overall, just need to add more narrative throughout the notebook. 
  + I like how you briefly state what each module is for and divide the notebook into different sections by steps. 


- Hui
  
Overall, your work on Task 3 is technically sound and follows the project requirements closely. You correctly cleaned the data, aggregated by Date, implemented time‑series cross‑validation, compared SLR and MLR models, and fit the best model to the full dataset. The workflow is clear and the results are reasonable.
+ Strengths:
  - Clear workflow and organization. Your notebook follows the same structure as the project instructions. This makes the notebook easy to follow.
  - Data cleaning matches the requirements. You removed the correct variables, aggregated by Date, and produced the expected number of daily observations.
  - Correct implementation of time series cross validation. Your helper function correctly trains on days ≤ _k_ and tests on day _k_ + 1, matching the sequential CV design.
  - Fitting the model correctly. You fit the MLR model to the full dataset and print coefficients, completing the final step of the task.
 
+ Suggestions for improvement:
  - Your introduction is very brief. It would be helpful to expand the introduction to explain the purpose of time-series cross-validation and the two models being compared.
  - Add more narrative around the data cleaning and expain the outputs. You perform the correct steps, but the narrative is minimal. Adding a short description of why you aggregate by Date and how this produces one observation per day would improve clarity. Give a brief explanation will be helpful for readers to better understand the results. 
  - Briefly explain the purpose of `day_arr`. You use `day_arr = pd.factorize(aq_df['Date'])[0]`. If you could explain how it creates a sequential day index and how it supports time-series cross validation, it would make this clearer.
  - Add doc strings to your helper functions. Your functions work well, but adding doc strings would improve readability.
  - Add a short discussion to compare SLR and MLR. You correctly state that MLR performs better, but you could expand slightly: Why do T, RH, and AH improve prediction? What does this suggest about the relationship between benzene and meteorological variables?
  - Minor formatting improvements, e.g., rounding outputs, adding comments, and consistent spacing would improve the readability of the notebook. Typo: `liek` should be `like`.

