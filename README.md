# Problem-Solving-with-Advanced-Analytics-by-Alteryx
This repository contains two projects which are part of Udacity's [Problem Solving with Advanced Analytics by Alteryx](https://www.udacity.com/course/problem-solving-with-advanced-analytics--ud976)

- [Predicting Diamond Prices](https://github.com/kartik-chandna/Problem-Solving-with-Advanced-Analytics-by-Alteryx/tree/master/predicting%20diamond%20prices)
- [Predicting Catalog Demand](https://github.com/kartik-chandna/Problem-Solving-with-Advanced-Analytics-by-Alteryx/tree/master/predicting%20catalog%20demand)

## Predicting Diamond Prices Project Details

A diamond distributor has recently decided to exit the market and has put up a set of 3,000 diamonds up for auction. Seeing this as a great opportunity to expand its inventory, a jewelry company has shown interest in making a bid. To decide how much to bid, the company’s analytics team used a large database of diamond prices to build a linear regression model to predict the price of a diamond based on its attributes. You, as the business analysts, are tasked to apply that model to make a recommendation for how much the company should bid for the entire set of 3,000 diamonds.

The following diagram represents the analysis at a high level. Since the model is already built, your analysis will focus on the right side of the diagram.

![](https://github.com/kartik-chandna/Problem-Solving-with-Advanced-Analytics-by-Alteryx/blob/master/predicting%20diamond%20prices/predictive-diagram.png)

The linear regression model provides an equation that you can use to predict diamond prices for the set of 3,000 diamonds. The equation is below:
<p align="center">
  <b>Price</b> = -5,269 + 8,413 x <b>Carat</b> + 158.1 x <b>Cut</b> + 454 x <b>Clarity</b></p>
<br/>

**Step 1 – Understand the data:** There are two datasets.

- **diamonds.csv** contains the data used to build the regression model.
- **new_diamonds.csv** contains the data for the diamonds the company would like to purchase

![](https://github.com/kartik-chandna/Problem-Solving-with-Advanced-Analytics-by-Alteryx/blob/master/predicting%20diamond%20prices/data-snapshot.png)

Both datasets contain carat, cut, and clarity data for each diamond. Only the _diamonds.csv_ dataset has prices. You'll be predicting prices for the _new_diamonds.csv_ dataset.

- _Carat_ represents the weight of the diamond, and is a numerical variable.
- _Cut_ represents the quality of the cut of the diamond, and falls into 5 categories: fair, good, very good, ideal, and premium. Each of these categories are represented by a number, 1-5, in the _Cut_Ord_ variable.
- _Clarity_ represents the internal purity of the diamond, and falls into 8 categories: I1, SI2, SI1, VS1, VS2, VVS2, VVS1, and IF. Each of these categories are represented by a number, 1-8, in the _Clarity_Ord_ variable

**Step 2 – Calculate the predicted price for diamond:** For each diamond, plug in the values for each of the variables into the linear model (equation). Then solve the equation to get the estimated, or predicted, diamond price.

**Step 3 – Make a recommendation:** Now that you have the predicted price for each diamond, it’s time to calculate the bid price for the whole set. Note: The diamond price that the model predicts represents the final retail price the consumer will pay. The company generally purchases diamonds from distributors at 70% of the that price, so your recommended bid price should represent that.

<br/>
<br/>

## Predicting Catalog Demand Project Details

You recently started working for a company that manufactures and sells high-end home goods. Last year the company sent out its first print catalog, and is preparing to send out this year's catalog in the coming months. The company has 250 new customers from their mailing list that they want to send the catalog to.

Your manager has been asked to determine how much profit the company can expect from sending a catalog to these customers. You, the business analyst, are assigned to help your manager run the numbers. While fairly knowledgeable about data analysis, your manager is not very familiar with predictive models.

You’ve been asked to predict the expected profit from these 250 new customers. Management does not want to send the catalog out to these new customers unless the expected profit contribution exceeds $10,000.

### Details

- The costs of printing and distributing is $6.50 per catalog.
- The average gross margin (price - cost) on all products sold through the catalog is 50%.
- Make sure to multiply your revenue by the gross margin first before you subtract out the $6.50 cost when calculating your profit.

Write a short report with your recommendations outlining your reasons why the company should go with your recommendations to your manager.

#### Steps to Success

##### Step 1: Business and Data Understanding

Your project should include:

- A description of the key business decisions that need to be made.

##### Step 2: Analysis, Modeling, and Validation

Build a linear regression model, then use it to predict sales for the 250 customers.You should create your linear regression model and come up with a linear regression equation.

Once you have your linear regression equation, you should use your linear regression equation to predict sales for the individual people in your mailing list.

##### Step 3: Writeup

Once you have your predicted or expected profit, write a brief report with your recommendation to whether the company should send the catalog or not.
