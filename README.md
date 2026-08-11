# StyleHub Sales Analysis

SQL and Power BI case study on two years of sales for StyleHub, a fictional clothing brand that sells online and in stores. The goal was to find out what sells best, when it sells the most, and where the business should focus next.

The work follows the six steps of data analysis: Ask, Prepare, Process, Analyze, Share and Act.

**Tools used:** SQL and Power BI

## A note about the data

This data is not from a real company. StyleHub is a made-up brand and the dataset was built to look like a real clothing business. It is used here to show analysis skills. No real customer data is used.

## Ask

In a real business the questions come from the stakeholders, the people who run the company. The analyst's job is to ask good questions first, so the goal is fully understood before touching the data. Asking the right questions early saves time and makes sure the analysis is useful.

StyleHub wanted to understand its sales and know where to focus next, so these were the key questions:

- What products sell the best?
- When does StyleHub sell the most during the year?
- Does the website or do the stores bring more sales?
- Which cities are the strongest?
- What should the business do next?

## Prepare

The data is a CSV flat file holding two years of sales, about 8,600 orders. Each row is one product in one order, with the date, city, price, cost and whether it was returned. I checked that the data had what was needed to answer the questions.

## Process

The raw data was messy, like real data always is. I cleaned it using SQL:

- Removed rows that were repeated
- Fixed category names spelled in different ways, for example "t-shirts" and "TSHIRTS" became one clean name
- Fixed city names with wrong spelling or spacing
- Marked blank cities and payment types as "Unknown" instead of deleting the sale
- Removed rows with zero or negative amounts, because those were mistakes

Then I added columns for revenue, profit and the month, so the data was ready to study.

## Analyze

1. StyleHub sells the most in winter. January is the biggest month, because the top products, Jackets and Boots, are for cold weather.
2. Shoes and Jackets make the most money, in both sales and profit. Accessories and T-Shirts sell a lot but earn very little.
3. Selling more does not mean earning more. The Baseball Cap sold the most units but made the least money, because it is cheap. Boots sold less but earned the most.
4. Most sales come from online, about 61 out of every 100 rupees.
5. Lahore and Karachi are the top cities, bringing almost half of all the money.
6. Every day of the week is about the same. People buy evenly all week.

## Share

To share what I found, I built a dashboard in Power BI. It shows sales by month, by product, by channel, by city and by day, with a filter to pick a year, so anyone can look at it and understand the business in one screen.

| Metric | Value |
| --- | --- |
| Total revenue | 37.9 million PKR |
| Total profit | 15.7 million PKR |
| Profit margin | about 41 percent |
| Total orders | 4,912 |

Dashboard visuals: revenue by channel (Online 60.55 percent, Store 39.45 percent), revenue by month, revenue by city (Lahore, Karachi, Islamabad), revenue by category (Shoes, Jackets, Jeans, Dresses, Kurtas, T-Shirts, Accessories), revenue by day of the week, and a year slicer.

## Act

In this final step I answer the questions the business asked at the start, and give my advice on what to do.

**What products sell the best?** Shoes and Jackets earn the most money, in both sales and profit. Accessories and T-Shirts sell a lot but earn very little. My advice: put the most money and effort into Shoes and Jackets, and use cheap items like Accessories to bring customers in, not to make profit.

**When does StyleHub sell the most during the year?** Sales are highest in winter, and January is the biggest month, because Jackets and Boots sell in the cold. My advice: stock up before winter, and spend the most on marketing in those months to make the most of the busy season.

**Does the website or do the stores bring more sales?** The website brings about 61 out of every 100 rupees, more than the stores. My advice: make the website the main focus, since that is where most sales happen.

**Which cities are the strongest?** Lahore and Karachi are the top cities, and together they bring almost half of all the money. My advice: focus delivery and marketing on Lahore and Karachi first, because that is where most customers are.

**What should the business do next?** Based on everything above, the biggest wins are in the top products, the winter season, the website and the two main cities. My advice: build stock and marketing around Shoes and Jackets before winter, push the online store hardest, and focus on Lahore and Karachi. This puts the effort where the money already is.

## Repository contents

Files to be added:

- SQL project used for the cleaning and analysis queries (stylehub_SQL.sqbpro)
- Power BI dashboard file
- Dashboard screenshot
- The Kaggle notebook version of this case study

## Links

- Kaggle notebook: https://www.kaggle.com/code/faizaninsights/case-study-for-e-commerce-brand
- Power BI file: add link
- SQL query: add link
