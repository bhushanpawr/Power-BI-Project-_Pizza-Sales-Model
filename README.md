# DASHBOARD
![Screenshot (90)](https://user-images.githubusercontent.com/113659167/210979361-ae1e0db0-d6ac-489c-8389-16d7d0f63318.png)

To find opportunities to increase sales and improve productivity, we have analysed the data in this PowerBI project and created a dashboard. At Plato's, things are going alright, but they could be better. For the past year, we have been gathering transactional data,  but really haven't been able to put it to good use.

Here are some questions that we solved in this project:

Q1 What days and times do we tend to be busiest?

Q2 How many pizzas are we making during peak periods?

Q3 What are our best and worst-selling pizzas?

Q4 What's our average order price?

Q5 What is the sales by category

### About Dataset

This dataset contain 12 columns are as below:

**Order id-** 
Unique identifier for each order placed by a table


**Order details id-** 
Unique identifier for each pizza placed within each order (pizzas of the same type and size are kept in the same row, and the quantity increases)


**Piza id-** 
Unique key identifier that ties the pizza ordered to its details, like size and price


**Quantity-** 
Quantity ordered for each pizza of the same type and size


**Order Date-** 
Date the order was placed (entered into the system prior to cooking & serving)


**Order Time-**
Time the order was placed (entered into the system prior to cooking & serving)


**Unit Price-**
Price of the pizza in USD


**Total Price-**
unit_price * quantity

**Pizza Size-**
Size of the pizza (Small, Medium, Large, X Large, or XX Large)


**Pizza Type-**
Unique key identifier that ties the pizza ordered to its details, like size and price


**Pizza Ingredients-**
ingredients used in the pizza as shown in the menu (they all include Mozzarella Cheese, even if not specified; and they all include Tomato Sauce, 
unless another sauce is specified)

**Pizza Name-**
Name of the pizza as shown in the menu

## 

Here i get a busiest time of the day by taking quantity and time of order and then plot it in a line chart.

conclusion of this visual is the time of a day at most pizza's are ordered around 13:00 and second peak of the day is between 17:00 to 19:00
![image](https://user-images.githubusercontent.com/113659167/210393907-99325320-693f-46fe-8207-34f310abff73.png)

##

In this visual i get a busiest day of the week by taking day-name and quantity of order. so i have created a new measure on order date column called "month name" by using **Day = FORMAT('Table'[order_date],"dddd")** this DAX formula.

Conclusion is that more pizza are ordered on Friday followed by Thursday and Saturday for the year.

![image](https://user-images.githubusercontent.com/113659167/210399196-9680c6ea-eaad-4034-beaa-dc5bb4acaf30.png)

##


