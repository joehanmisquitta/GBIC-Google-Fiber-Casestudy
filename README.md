# GBIC-Google-Fiber-Casestudy

I used the following SQL query in Google BigQuery to create a single combined table that merged all three of the given datasets 
The UNION ALL statement is applied here instead of a JOIN statement because the tables already have matching columns, making them easy to merge completely.


'''sql
SELECT date_created, contacts_n, contacts_n_1, contacts_n_2, contacts_n_3, contacts_n_4, contacts_n_5, contacts_n_6, contacts_n_7, new_type, new_market FROM `your project.fiber.market_1`;
UNION ALL
SELECT date_created, contacts_n, contacts_n_1, contacts_n_2, contacts_n_3, contacts_n_4, contacts_n_5, contacts_n_6, contacts_n_7, new_type, new_market FROM `your project.fiber.market_2`;
UNION ALL
SELECT date_created, contacts_n, contacts_n_1, contacts_n_2, contacts_n_3, contacts_n_4, contacts_n_5, contacts_n_6, contacts_n_7, new_type, new_market FROM `your project.fiber.market_3`;
'''
 
## Vistualization 

The Following Visualizations were created in Tableau from the combined market data set

![Dashboard 1](https://github.com/joehanmisquitta/GBIC-Google-Fiber-Casestudy/assets/62551712/c9c6d07a-4ca5-41d6-9fca-5a871e71c7d8)


![Dashboard 2](https://github.com/joehanmisquitta/GBIC-Google-Fiber-Casestudy/assets/62551712/ec1e077e-9dcf-49f4-b146-75a162f57f47)
