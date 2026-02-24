Each group member should provide feedback on the other group members’ work. Be detailed and specific where possible. The quality of this feedback can play a part in your grade.

You can provide feedback to your group members in many different ways (live in a meeting, offline, or however else you devise) but the feedback must be documented here! 

Please replace “Feedback giver #x” with a group member’s name below and add feedback as a bulleted list below. Note: There is a pencil icon on the top right of the README file (when you are viewing the README.md file) that allows you to edit.

- Hui Fang
  
Good job on Task 1, Bing! Your work is technically solid, well structured, and complete for Task1. You implemented all required components — grid search, gradient descent (constant and SLR), RMSE functions, difference quotients, and comparisons with `SciPy`. The structure is clear, the code runs clearly, the logic is easy to follow, and the results match theoretical expectations. This shows you have strong understanding of numerical optimization and simple linear regression. Below are some detailed comments to help improve your task even further. 
+ Strengths:
   +  The introduction is concise but informative. It gives readers a clear sense to understand what the project will cover and sets up the workflow.
   +  The data clear steps are clear with good explanations. You show what you removed and why, and the before and after shapes help readers understand the impact.
   +  In the Prediction of C6H6(GT) section, the definitions of squared error loss and RMSE equation are very helpful. Including the formulas makes the mathematical foundation explicit and accessible.
   +  Your function definitions are well organized. Listing parameters and documenting them makes the code easy to follow.
   +  The overall flow is logical and easy to navigate.
   +  After revisions, you incorporated the feedback to refine the notebook. The introduction provides more an overview of the task, the added section narrative guide reader easily to follow. The takeaways highlights the practical differences between grid search and gradient descent, and shows that adding relevant explanatory variables generally leads to a better‑fitting model.
+ Suggestions for improvement:
   +  Add more narrative throughout the notebook to explain your reasoning, interpret results, and guide the reader.
   +  Add brief comments explaining your choices of step sizes, starting values, and tolerances. e.g., why do you choose Q1 – Q3 for the grid, why start β<sub>0</sub> at -20, why choose step sizes of 0.5 and 0.000005, why use tolerance 0.00001?
   +  Fix a small notation issue in the RMSE formula. In the RMSE equation, the summation uses 𝑦<sub>1</sub> , but it should be 𝑦<sub>i</sub>.
   +  Clarify the two modeling cases. In the two cases, it could be clearer if you clarify case 1: we only use the response variable to estimate the constant c; case 2: we model c as a linear function of one numeric predictor: _c_ = β<sub>0</sub>+β<sub>1</sub>x. This helps readers understand the conceptual jump from constant prediction to simple linear regression.
   +  Avoid printing all 1000 RMSE values. For _c_ in c_grid, instead of printing out all 1000 values, it could be better to print just a few, e.g., `rmse_values[:10]`. Or you can add a plot to show distribution of RMSE.
   +  Round key outputs for readability: It could be better for some of the key values, e.g., grid search β<sub>0</sub> and β<sub>1</sub>, if you can round up to 4 decimal places for clarity: `print(f"(b0, b1) = ({best_b0: .4f}, {best_b1: .4f}) is the optimal linear prediction!")`.
   +  Provide brief comments explaining the main steps of your code. Your code it correct, but adding short comments to some will help readers follow the logic more easily, especially those less familiar with numerical optimization.
   +  Add a short comparison between grid search and gradient descent. Since you implemented both methods, a concise summary would be helpful. For example, whether the two methods converged to similar estimates, which one is easier to implement, etc.

- Cole Hammett
  
  	I do not have a strong background in calculus but I have been introduced to gradient descent algorithms because I use neural networks in my research. I will do what I can to offer constructive comments to your submission! Just as a basic overview, you did a good job of following the good programming practices. Your markdown comments are well thought out. You included multiple steps in one block of code where I broke mine up into very small lines. However, the effect is the same because your markdown describes all parts of the code.
  
  	I like your very thorough explanation of the staistics with equations and all! Please consider easing into this a little slower would be one recommendation to consider. Some readers might know what you're talking about here with these terms but someone who only knows basic statistics might sturggle. For example:
	+ What is your motivation? Why are you trying to predict this value?
	+ What are the consequences of low quality predictions? What are the stakes?
  	+ What are other examples of loss functions?
  	+ What question are you answering with this section? How will you know if your answer is valid?
  	  
  	Your code is very neat and tighty. The way you right combines many steps into minimal lines of code. It's all very pythonic! I like that you include many inputs into your arguments rather than just hardcoding them for only this assignment.
  
  	At the end of each section, consider adding a block of markdown talking about what the takeaways are.
  	+ Do you think this method was very effective? How easy was it to develop?
  	+ What other types of data could this workflow be used for?
  	+ What is the signficance of the predictions in the context of the experiment?
 
  	I like how you added ideas on how the process could be improved upon, such as how one could modify the input parameters into the function and potentially see better results (markdown between cells 28 and 29). There is a difference in the workflow at the very end of your two sections. When you are estimating for specific input variables, you use arithmetic to calculate these from the equation for the regression line. In the grid search section, you copy and pasted the numeric value of the coefficients and did your calculation that way. In the gradient descent section, you stored the return of the function (the coefficients) as variables then used those to calculate the estimates. They both give the same output so functionally it isn't important but it maybe something to consider for consistencies sake. 
 

 
  	  
	
  
