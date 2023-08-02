# Project1: Netflix User EDA
Instructor:  Steven Greene  
Bootcamp:  DU-VIRT-DATA-PT-06-2023  
2 August 2023  

## Table of Contents
- [About](#about)
- [Questions](#questions)
- [Contributing](#contributing)
- [Resources](#resources)
- [Presentation](#presentation)
- [Results](#results)
- [Summary](#summary)
  
## About
A Netflix dataset from Kaggle was used to analyze Netflix user demographics, consumption patterns, subscription preferences, and turnover rates across ten different countries including Australia, Brazil, Canada, France, Germany, Italy, Mexico, Spain, United Kingdom, and United States.

## Questions
- Who are Netflix’s users? Age, Distribution, Gender. (Jennifer)
- How are Netflix's users consuming content? Mobile, Desktop, Laptop, TV. (Juliet)
- How much revenue is Netflix generating from its users? Revenue Distribution by Country. (Ryan)
- What is Netflix’s Turnover Rate and Average Subscription Length? The turnover rate, as defined by users who were active for less than 31 days. (Adam)

## Contributing
- <a href="https://www.github.com/zonaj2/" target="_blank">Juliet Hamilton</a>  
- <a href="https://www.github.com/jgrubb38/" target="_blank">Jennifer Grubb</a>  
- <a href="https://www.github.com/agostinger/" target="_blank">Adam Gostinger</a>  
- <a href="https://www.github.com/ryguy57/" target="_blank">Ryan Himes</a>  

## Resources
- <a href="https://www.kaggle.com/datasets/arnavsmayan/netflix-userbase-dataset" target="_blank">Netflix User Dataset</a>  

## Presentation
- <a href="https://docs.google.com/presentation/d/1U1dDa6DbaJYQS9jKfR0n--EW8HZvPx9mpKCgl28FO5A/edit?usp=sharing" target="_blank">Google Slide Presentation</a>

## Results
### Who are Netflix’s Users?
A break-down of Gender and Age was performed to see the typical Netflix customer out of the dataset that includes 2500 users.
<p align="center">
<img src="https://github.com/zonaj2/Project1/blob/main/images/gender_chart.png">  
</p>  
The analysis shows that there is a near-even balance between females and males from the 10 countries in the dataset: Australia, Brazil, Canada, France, Germany, Italy, Mexico, Spain, United Kingdom, and United States. 
<p align="center">
<img src="https://github.com/zonaj2/Project1/blob/main/images/ages_chart.png">  
</p>  
The analysis shows the majority of Netflix users fall within the age range of 31 - 50. This analysis aligns with the trends in media consumption and internet usage. There are several reasons that could contribute to this age distribution; time availability, family and lifestyle, content preferences, and social influence.  

### Netflix Customer Content Consumption
Netflix users access the platform through a wide range of devices.  This dataset focused on the following devices: Smart TV, Laptop, Smartphone, and Tablet.
In the study, the 2500 Netflix users exhibited a uniform distribution across the four device types, with each device type accounting for approximately 25% of the total usage count.
Within device type the category of Gender was analyzed.  Gender is defined as those identifying as either Male or Female. The results showed that Gender is equally divided among: Smart TV, Laptop, and Tablet.  There was a slight gender difference in the Smartphone usage, with males having a slightly higher percentage of use compared to females. Males, smartphone – 82%, Females, smartphone – 28%.  
<p align="center">
<img src="https://github.com/zonaj2/Project1/blob/main/images/pie_device_gender.png">  
</p>  
Exploring the relationship between smartphone usage by males and females for watching Netflix, specifically focusing on screen size differences, can be an interesting analysis. My guess is that:  

1. Males often tend to use smartphones with larger screen sizes for watching Netflix, possibly influenced by the fact that most pockets on men's clothing can better accommodate bigger phones.  
2. Females, on the other hand, may prefer smartphones with smaller screen sizes for accessing Netflix, as the pockets on their clothing are often less spacious and not as suitable for carrying larger devices.  

The device used to consume Netflix content doesn't seem to have a high impact on the monthly revenue per user, suggesting that Users' device choice is independent of the amount they spend on Netflix each month.  
<p align="center">
<img src="https://github.com/zonaj2/Project1/blob/main/images/box_revenue_device.png">
</p>  

Within each country there seems to be an even distribution for the count of Laptop, Smart TV, Smartphone, and Tablet.  
<p align="center">
 <img src="https://github.com/zonaj2/Project1/blob/main/images/device_country.png">  
 <img src="https://github.com/zonaj2/Project1/blob/main/images/Screen%20Shot%202023-08-01%20at%205.49.00%20PM.png">  
</p>  

### Netflix Revenue By Country and Subscription Type Analysis
Netflix's revenue distribution by country is a crucial aspect of its business strategy, as it provides insight into the contribution of different countries to its overall revenue. The data analysis enables Netflix to target investments in specific markets and regions, bolstering its revenue.  
The analysis comprises two main visualizations, a pie chart, and a stacked bar chart. The pie chart presents an overview of revenue distribution by country, clearly showing each country's contribution to Netflix's global revenue landscape. The United States and Spain lead with 18.1% of total revenue, closely followed by Canada with 12.6%. The remaining seven countries, including the United Kingdom, Italy, France, Brazil, Australia, Germany, and Mexico, each contribute 7.4% and 7.2% of the total revenue.  
<p align="center">
<img src="https://github.com/zonaj2/Project1/blob/main/images/Pie_Chart_Revenue_Distribution.png">
</p>  
The stacked bar chart summarizes each country's monthly revenue, categorized by subscription types, basic, premium, and standard. This chart enables Netflix to understand which subscription types generate the most revenue in each country and identify revenue patterns and trends. The insights from this chart assists in making data-driven decisions to optimize revenue generation strategies.  
<p align="center">
<img src="https://github.com/zonaj2/Project1/blob/main/images/Stacked_Bar_Chart_Total_Monthly_Revenue.png">
</p>  
The United States stands out as the top revenue-generating country for the basic subscription type, with Italy and Germany also contributing significantly. On the other hand, France, Australia, Mexico, and the United Kingdom have relatively minimal revenue contributions from the basic subscript and type.  
Regarding the premium subscription type, Spain leads in revenue contribution, with France and the United States also making substantial contributions. Australia and Canada show moderate revenue, With Brazil, Italy, and Germany contributing relatively less. Notably, the premium subscription type has no revenue in Mexico or the United Kingdom.  
The United Kingdom and Mexico are the top revenue contributors for the standard subscription type, with the United Kingdom showing the highest revenue among all countries and subscription types. Spain and the United States followed with significant contributions. Canada, Australia, and Germany have moderate revenue contributions, while Brazil and Italy show relatively more minor revenue. The standard subscription type has no revenue in France.  
Together these visualizations provide a comprehensive understanding of Netflix's revenue landscape, enabling informed decision-making, effective market prioritization, and tailored services for specific regions. By analyzing global performance, identifying growth opportunities, and driving strategic decisions, Netflix can ensure its streaming services' long-term success.  

### Netflix Customer Turn-Over Rate
Customer turnover rate is the percentage of an organization's customer base lost during a certain time period. A high turnover rate can result in reduced revenue and profitability.
In order to estimate Netflix’s customer turnover rate within the dataset, customer turnover was defined as customers who left the company on or before 31 days of service (1 Month). This was performed by subtracting the customer join date from the latest customer payment date. These dates were converted to proper format in order to calculate days subscribed and months subscribed. The data was then filtered for customers who subscribed for 31 days or less. The turnover percentage was calculated based on the number of customers subscribed for 31 days or less divided by total customers.  
The customer turnover rate is only .24% of customers within this data suggesting Netflix has a very low customer turnover rate with an average subscription of about 11 months. The low turnover rate suggests most customers use Netflix past the first month and are satisfied with the service.  

### Netflix Average Subscription Length and Turnover by Age Group
In order to further analyze the data for customer turnover and subscription length, age groups were created based on the age of the customer using the Netflix service. The age groups used were less than 30, 30-35, 35-40, 40-45, 45-50, and 50+ years old. This provided an even dataset across the age groups. The age groups were used to calculate an average monthly revenue, average months subscribed and turnover rate for each group.  
The data based on the age groups was graphed to compare age versus average monthly revenue and average months subscribed using a line graph. The line graph and data suggest that the higher the age, the less months the customers stay subscribed, and less revenue is being generated by Netflix. This could be due to older generations typically being more resistant to technology (i.e., subscribing to cable as opposed to streaming platforms such as Netflix) compared to younger generations who prefer streaming. A follow-up analysis to compare age to cable users vs. streaming users could be useful to support this further.  
<p align="center">
<img src="https://github.com/zonaj2/Project1/blob/main/images/Age_Rev_Months.png">
</p>  
Further evidence of age being a factor in Netflix’s customer turnover and therefore revenue was shown by plotting the turnover rate on a pie chart. The pie chart presents customer turnover based on age group. The largest turnover was in the 40-45 age range.  While Netflix turnover rate overall is very low, the majority of turnover (67%) was the result of the 40-45 age group.  
<p align="center">
<img src="https://github.com/zonaj2/Project1/blob/main/images/Turnover_AgeGroup.png">
</p>  
Lastly, a Pearson correlation calculation and regressive line plot was used to determine how strong the relationship is between average days subscribed and the customer age group. The Pearson correlations range from -1 to 1 with 0 implying no correlation. The correlation of -0.78 suggests a strong negative relationship between months subscribed and age. As the age increases, the average months a user is subscribed is decreasing. Again, this could be due to the older generation being more resistant towards change and technology than the individuals under age 30. This knowledge of age group could help Netflix better target the older generation in order to keep them as customers longer, which would result in increased revenue.  
<p align="center">
<img src="https://github.com/zonaj2/Project1/blob/main/images/Correlation.png">
</p>  

## Summary
The analysis of Netflix's customers including location, gender, subscription type, monthly revenue, how content is consumed, and  length of time subscribed provided an insight into Netflix's business  and potential areas for improvement.  
  
User Demographics: Netflix boasts a diverse global customer base with users in Australia, Brazil, Canada, France, Germany, Italy, Mexico, Spain, United Kingdom, and United States. The majority of Netflix users fall within the age range of 34-54 years old and is evenly balanced between females and males from the 10 countries.  
  
Content Consumption: Netflix customers in all countries analyzed utilize content fairly evenly across laptops, smart TVs, tablets and smartphones, with about 25% in each type. While gender was mostly even across all devices, there was a slight preference amongst men for watching content on a smartphone. Users' device choice does not impact the amount spent on Netflix each month.  
  
Revenue Generation: The United States, Spain and Canada are the top three revenue-generating countries across all subscription types. The Premium subscription type has no revenue from Mexico or the United Kingdom but are the top revenue contributors for the Standard subscription type.  
  
Customer Turnover Rate and Months Subscribed: The turnover rate was 0.24% based on customers who unsubscribed on or before 31 days, and mostly amongst 40 or older. The average months subscribed trended lower with age suggesting lower engagement with the older audience. Overall, the data suggests that Netflix retains a majority of its customers with potential to target the more mature viewers.  
  
In conclusion, the insights gained from this analysis can help guide Netflix in strategic decision-making to increase users, enhance engagement, and increase revenue for Netflix.  
