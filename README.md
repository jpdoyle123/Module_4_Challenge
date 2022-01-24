# Module_4_Challenge

In this challenge, we were tasked with analyzing a portfolio of stocks in numerous different manners, such as beta, covariance, standard deviation, as well as the rolling varieties of each of these analytic tools. 

<img width="978" alt="Screen Shot 2022-01-23 at 7 52 48 PM" src="https://user-images.githubusercontent.com/95647683/150705890-94442e2c-215d-4c85-be0b-a3b0983a9570.png">

This section is where we imort the needed libraries for our code. These are the numpy, Path, and Pandas libraries. Underneath is where we read in the whale_navs.csv file located in the Resources folder of this repository. The first five rows are shown as well. 
<img width="910" alt="Screen Shot 2022-01-23 at 7 55 52 PM" src="https://user-images.githubusercontent.com/95647683/150705986-72fbc22e-e750-4f1a-a3b6-585889ee87f9.png">
Here we use the pct_change function as well as the dropna function to convert our data to daily returns, reason being that daily returns are a much more honest metric to use when calculating risk, as there is no problem of scale differences. 

The next section is the first of our quantitative analyses. 
<img width="977" alt="Screen Shot 2022-01-23 at 7 57 28 PM" src="https://user-images.githubusercontent.com/95647683/150706130-beb64aec-0fd0-4df7-92f7-1128dbaa1a40.png">
<img width="968" alt="Screen Shot 2022-01-23 at 7 57 38 PM" src="https://user-images.githubusercontent.com/95647683/150706142-acba2578-fa1d-48d5-9f6f-984ba3a201c2.png">
<img width="966" alt="Screen Shot 2022-01-23 at 7 57 47 PM" src="https://user-images.githubusercontent.com/95647683/150706150-5fdbafd8-9867-4e60-acf9-c9a0ccd87d33.png">

The first picture is of a plot of our daily returns data for each stock. The second is a screenshot of our code for calculating cumulative returns for each stock, which is then plotted in the third screenshot. As we can see, the returns of these stocks do not seem to outperform the S&P 500, just based on cumulative returns. However, we can see some more volatility that will be explored next. 

<img width="966" alt="Screen Shot 2022-01-23 at 7 57 47 PM" src="https://user-images.githubusercontent.com/95647683/150706240-2ac43ce1-f6d9-46b1-a57a-43d60a4af758.png">
This screenshot shows the box plots for the different stocks. As we can see, the S&P 500 has much higher volatility compared to any of the stocks. 
<img width="977" alt="Screen Shot 2022-01-23 at 8 01 12 PM" src="https://user-images.githubusercontent.com/95647683/150706304-20a1b06c-025e-4358-b631-73ce839c3a1e.png">
<img width="925" alt="Screen Shot 2022-01-23 at 8 01 19 PM" src="https://user-images.githubusercontent.com/95647683/150706308-4c250fd8-d6a5-402c-8156-fb7b4e84a826.png">
<img width="958" alt="Screen Shot 2022-01-23 at 8 01 31 PM" src="https://user-images.githubusercontent.com/95647683/150706311-275c4c0c-ebc7-4922-8d7b-3690d80e438c.png">

The first screenshot above shows our standard deviation calculations for each of the four stocks and the S&P 500. We can see that, after annualizing these numbers, that the S&P is the most volatile, while Tiger is the least volatile. The following two screenshots show the annualized standard deviation over a 60 day rolling period. Besidesthe S&P 500, Berkshire Hathaway presents the most volatility. 

<img width="915" alt="Screen Shot 2022-01-23 at 8 03 57 PM" src="https://user-images.githubusercontent.com/95647683/150706429-0a4397ed-fe54-4cd0-b505-7c66251771a0.png">
<img width="765" alt="Screen Shot 2022-01-23 at 8 04 13 PM" src="https://user-images.githubusercontent.com/95647683/150706438-0df386c3-7af3-4f27-bb4b-6490b43c6031.png">

These screenshots show the calculation of the sharpe ratios for each stock. Looking at the bar graph, we can see that Berkshire Hathaway, according just to sharpe ratios, has the best risk-return profile. 

Next, we calculated rolling beta for two stocks: Berkshire Hathaway and Tiger Global Management. 

Data for Berkshire Hathaway:
<img width="917" alt="Screen Shot 2022-01-23 at 8 06 18 PM" src="https://user-images.githubusercontent.com/95647683/150706587-babebb57-c445-4cfc-9d67-a0eba165b3dd.png">
<img width="914" alt="Screen Shot 2022-01-23 at 8 06 29 PM" src="https://user-images.githubusercontent.com/95647683/150706607-7ea96d45-6fa8-4275-ab12-1af33f70493c.png">
<img width="929" alt="Screen Shot 2022-01-23 at 8 06 35 PM" src="https://user-images.githubusercontent.com/95647683/150706612-8f1d427e-b9c7-44f1-80af-d4c3b2e0e497.png">
<img width="911" alt="Screen Shot 2022-01-23 at 8 06 45 PM" src="https://user-images.githubusercontent.com/95647683/150706624-7e3bd5b8-f5b4-4f84-bdb0-2a3d3fb476cf.png">
<img width="936" alt="Screen Shot 2022-01-23 at 8 06 53 PM" src="https://user-images.githubusercontent.com/95647683/150706628-20466d7f-f95f-48ce-bf13-948628de2dd3.png">

Data for Tiger Global Management:

<img width="968" alt="Screen Shot 2022-01-23 at 8 09 18 PM" src="https://user-images.githubusercontent.com/95647683/150706697-d267b2a8-6f1e-4b89-a2f1-41ea3e401790.png">

<img width="970" alt="Screen Shot 2022-01-23 at 8 09 25 PM" src="https://user-images.githubusercontent.com/95647683/150706702-5d446530-577a-4232-bb57-0e1d68a7fe1b.png">
<img width="968" alt="Screen Shot 2022-01-23 at 8 09 32 PM" src="https://user-images.githubusercontent.com/95647683/150706707-d848b844-d603-4687-a43e-5f69885b542d.png">
