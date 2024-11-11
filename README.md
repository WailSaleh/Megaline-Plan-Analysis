# Megaline-Plan-Analysis 🌐📱

An analysis will be conducted for the telecommunications company Megaline, which offers two prepaid plans: Surf and Ultimate. A preliminary examination will be carried out using a sample of 500 customers. Data will include information on who the customers are, their locations, the plan they use, and the number of calls and messages made in 2018.

Here is a breakdown of the plans:

**Surf**
Monthly price: $20
500 minutes per month, 50 text messages, and 15 GB of data
After exceeding the packet limits:
1 minute: 3 centavos
1 text message: 3 cents
1 GB of data: $10

**Ultimate**
Monthly price: $70
3,000 monthly minutes, 1,000 text messages, and 30 GB of data
After exceeding the packet limits:
1 minute: 1 centavo
1 text message: 1 cent
1 GB of data: $7

The goal is to determine which plan generates more revenue to help adjust the advertising budget effectively.

The analysis process is as following:
1- Organize and clean the data in order to have a clear analysis.
2- Analyze the usage patterns of customers on both plans, including the number of calls, minutes, messages, and internet usage.
3- Calculate and compare the revenue generated by each plan based on its pricing structure.
4- Provide insights and recommendations based on the analysis to determine which plan is more profitable for Megaline.

In this project, will work with five separate tables.

**users:**
user_id — unique user identifier
first_name — username
last_name — user's last name
AGE — user's age (in years)
reg_date — date of registration (dd, mm, yy)
churn_date—the date the user stopped using the service (if the value is missing, it means that the plan was in use when the database was extracted)
city — user's city of residence
Plan — Plan name

**calls:**
ID — Unique caller ID
call_date — date of the call
Duration — call duration (in minutes)
user_id — identifier of the user making the call

**messages:**
id — unique identifier of the text message
message_date — date of text message
user_id — identifier of the user who sends the text message

**internet:**
ID — unique identifier of the session
mb_used — volume of data spent during the session (in megabytes)
session_date – date of the web session
user_id - user identifier

**plans:**
plan_name — plans name
usd_monthly_fee - monthly price in US dollars
minutes_included — monthly minutes package
messages_included — monthly text messaging package
mb_per_month_included — volume of the data packet (in megabytes)
usd_per_minute – price per minute after exceeding the bundle limit (e.g., if the bundle includes 100 minutes, the first excess minute will be charged)
usd_per_message – price per text message after exceeding the package limit
usd_per_gb – price per extra gigabyte of data after exceeding the packet limit (1 GB = 1,024 megabytes)

