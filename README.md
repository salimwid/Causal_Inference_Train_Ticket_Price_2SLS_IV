# Causal_Inference_Train_Ticket_Price_2SLS_IV
Adopted 2SLS and Instrument Variable to solve the endogeneity problem in predicting train ticket price.

#### Techniques Employed
Two-stage least square (2SLS), Instrumental Variables, Econometrics, Linear Regression <br>

### Context
In this project, the demand function for trains using train ticket sales data is estimated at a particular train station. The problem is complex by nature as the demand function can never be estimated without complication due to simultaneity of the supply and demand functions. As such, we approached the problem of estimation by adopting the Two-Stage Least Squares (2SLS) regression model. The 2SLS model allows us to eliminate endogeneity bias which would be prevalent in the Ordinary Least Squares (OLS) model of a demand function. <br>

### Dataset
The datasets used were of train ticket sales data from June 2018 to June 2019. The datasets present 209,697 entries and 14 distinct features. Each entry represents a ticket purchase within the time period. <br>

### Implications & Insights
By estimating ln(price) with cabin type, we have removed the hidden variables affecting price from this model. The chosen IV model passed all the endogeneity tests and we found that the original OLS model indeed suffered from endogeneity bias. <br>

The coefficients of all the variables used in both the IV and 2SLS models are in line with our understanding and business applications - as described in part 4.3. Thus, the final 2SLS model seems to have solved the endogeneity problem posed by the original OLS model. Nonetheless, the model has a large
residual as evident in the low adjusted R-squared, and as such, there is room for potential improvements. <br>

### Collaborators
Kyle Kenji Asano (@kasano)<br>
Widya Salim (@salimwid)<br>
Sae Jin Jang (@saejin123)<br>
Hpone Myat Khine (@HponeMK) <br>
Amy Mingxuan Yang (@mingxuanyang-amy)
