# E-Commerce-Clients

## About the data

Data containing information about :     

*	InvoiceNo
*	StockCode
*	Description
*	Quantity
*	InvoiceDate
*	UnitPrice
*	CustomerID

Data contains `4,371` users that will be categorize based on their purchase history. The category will be divided into 3 type of customers with detail such as :
### Long Period Users 
The requirement :  
- Users do more than or equal to 7 (round up average of invoce count) transaction / invoice and have different date between 1st invoice date with the last invoice date,
- Users average date must be more than or equal to `25 days 10:43:18.160874013` (Average of average date)

### Short Period Users
The requirement :  
- Users do more than or equal to 7 (round up average of invoce count) transaction / invoice and have different date between 1st invoice date with the last invoice date,
- Users average date must be less than `25 days 10:43:18.160874013` (Average of average date)

### Big Buyers Users 
The requirement :  
- Users with more than 0 Qty purchase, and more than 1 invoice.
- With minimal purchase at `1133.58` (Average of Qty)


## Goals : 
- Revenue Trend
- Average Revenue Trend Per User
- Month to Month Average Revenue Trend
- Identify Customer By Purchase History
- Identify Big Buyer Customer

## Result

### Based on the data `Revenue trend per month` :
- The lowest revenue is on `11-2018` with `104,842.84`
- The highest revenue is on `11-2019` with `1,496,272.65`

### The result of `Average revenue trend per user` :     
- The average revenue is on `35.82`
- The lowest revenue is on `26.72`
- The highest revenue is on `50.01`

### The result of `Month to month revenue trend` :
- The average number is on `33.81`
- The minimal is on `24.84`
- The maximal is on `41.22`

### Here's some analysis about `Long period of time buyer` :
- From Scatter Plot, Customer with more invoce tend to buy faster.
- There're `435` users with average invoice at `8.94` invoices
- Average time of buying between 1 invoice to another is `35 days 02:40:50.757835268`

### Here's some analysis about `short period of time buyer` :
- The more invoices customer the shorter time customer use to do another purchase.
- There're `456` users with average invoice at `21.390351` invoices
- Average time of buying between 1 invoice to another is `16 days 05:26:41.933509658`

### Here's the analysis result from Big Orders :
- From Scatter Plot, Customer tend to do repeat order, with a big amount of qty. The less invoice customer has the more qty customer order.
- From `920` Customers, with average result of `13.58` invoice dan average qty `323.96`

### Hypothesis Result
I analyst 2 hypothesis, here is the details of the hypothesis : 
- Hyphothesis 1 :
  - `H0 = There're no differences in average order frequency and size for different user segments`
  - `H1 = There're differences in average order frequency and size for different user segments`
  - The result after the testing is `We reject the null hypothesis (H0)`
- Hyphothesis 1 :
  - `H0 = There're no difference between average revenue by item on member and non member`
  - `H1 = There're difference between average revenue by item on member and non member`
  - The result after the testing is `We reject the null hypothesis (H0)`
 
### [Dashboard](https://public.tableau.com/views/Final_17096962377890/E-Commerce?:language=en-US&publish=yes&:sid=&:display_count=n&:origin=viz_share_link)
### [Presentation](https://docs.google.com/presentation/d/1UsgiLBn4zjuHi4VuhmH5AdGqzd-hnlntrBQZ4_rFbsk/edit?usp=sharing)
