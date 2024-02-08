
# Meal delivery optimization-Dashboard


## Problem Statement


The client is a meal delivery company that operates in multiple cities. They have various fulfillment centers in these cities for dispatching meal orders to their customers.The client wants to help these centers with demand forecasting for upcoming weeks so that these centers will plan the stock of raw materials accordingly.

The replenishment of most raw materials is done on a weekly basis and since the raw material is perishable, procurement planning is of utmost importance.

The client wants and end to end report to understand which fulfillment areas are doing well and which are not.


#### We have the below information with us in the form of 3 different datasets:

- Historical data of demand for a product-canter combination

- Product (Meal) features such as category, sub-category, current price, and discount

- Information for fulfillment centers like center area, city information, etc.

## Steps Taken

 The problem statement lacked a specified date or time period, relying solely on weeks (1 to 145), equivalent to approximately 2.7 years.

 To address this, we engineered a virtual calendar using CALENDAR(), spanning from January 6, 2019, to October 24, 2021—roughly correlating with the provided 145-week range.

 This virtual calendar was linked to a new Date table. This auxiliary table, featuring details beyond week numbers (e.g., months, quarters), established a many-to-many cardinality with the Weekly_Demand_Data table.

 Leveraging the Date table, we implemented a dynamic Date filter in our dashboard, empowering users to explore data across various temporal dimensions such as Years, months, and quarters.


        We have come up with a story in Power BI that talks about the level of demand in each center. 
        This analysis is granular enough to include product information as well.


#### The Dashboard answers some major questions like

- What is the total number of orders catered by the firm?
  
![image](https://github.com/Yaszh/meal_delivery_dashboard/assets/71252244/28935903-906c-42d5-ab8e-ece360f39e1d)

- What is the revenue earned by the firm?
  
![image](https://github.com/Yaszh/meal_delivery_dashboard/assets/71252244/a421677e-b265-4eba-8241-ab8bead1d952)

- What is the total discounted value
- What is the overall discount %?
![image](https://github.com/Yaszh/meal_delivery_dashboard/assets/71252244/e8f0a951-7a74-49af-b895-48d7806fc976)



![image](https://github.com/Yaszh/meal_delivery_dashboard/assets/71252244/6b92158e-cdd0-4eb0-977b-a7203c8f6223)


 The overall analysis also includes a scatterplot. This scatter plot visualizes the correlation between the number of orders and revenue, categorizing meals. Each dot represents a meal order, with the X-axis indicating the order count and the Y-axis reflecting revenue. The legend differentiates meal categories, offering insights into their performance. Additionally, the play axis introduces a temporal dimension, enabling a dynamic view across quarters for a comprehensive analysis of sales trends over time.

 Additionally, the main page features a versatile date filter, enabling users to explore data by Year, Quarter, and Month. This interactive feature enhances the analysis, providing a granular view of sales trends based on selected time parameters.

### Apart from that the main page involves 4 buttons that redirects the user to various visuals each representing an important analysis.

- Top categories
![image](https://github.com/Yaszh/meal_delivery_dashboard/assets/71252244/0e28c8df-ce43-4364-9fe1-dd20091312c1)

- Op-area Influence
![image](https://github.com/Yaszh/meal_delivery_dashboard/assets/71252244/1b8a9987-a5aa-41d8-8029-b61e0208319e)

This insight is provided with the help of *Key Influencer* chart. It cal also explain the Operational area influnce based on increasing number of orders by simply clicking on the drop at the top and change it to Increase.

- Promotional Activities
![image](https://github.com/Yaszh/meal_delivery_dashboard/assets/71252244/98f27b62-74c8-4d59-b8d4-01eda95481a7)


Through this visuals the stakeholders could understand whether the emails & product features on the homepage an effective mode of promotion as it includes the number of orders for each category as well

- Forecasting

![image](https://github.com/Yaszh/meal_delivery_dashboard/assets/71252244/e1e53762-bce5-40c1-b350-67c2c10cc02a)





