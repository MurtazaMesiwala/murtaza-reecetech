# BI Engineering Homework Assignment
Thank you for taking the time to tackle this assignment. We've tried to create a scenario that reflects the sorts of challenges you'll be working on here. **It is important that you read the context and instructions that follow**. Enjoy!

## About Data & AI at Reece
Data & AI at Reece is at an inflection point that reflects Reece’s growth over the last century supporting trade industries and improving the lives of our customers and people every day. We are known for an unparalleled, human understanding of our customers — and we have a clear, long-term vision for becoming trade’s most valuable partner, helping them succeed in a digital world.

## About Our Branch Operations
Reece’s branch operations are at the heart of our customer experience. Our branch teams regularly engage in detailed customer relationship development meeting cadences with our Trade customers to understand their businesses, and co-develop approaches to helping them succeed — these activities negotiate wide range of topics such as how pricing, logistics, merchandising, product lines and other services can be tailored to help our customers run their businesses more successfully. Our branch teams leverage our customers transaction information through our in-house point of sale system (The Reece System, TRS), as well as tools such as Salesforce Customer 360 and PowerBI reporting to make sense of customers’ interactions with Reece to inform who they should be talking to, for what specific purpose (e.g. marketing, relationship development, operating/commercial activities such as navigating of credit arrangements on occasion required).

## Instructions for this assignment
One area Reece is considering offering enhanced service to our customers is in assisting them with meeting their credit account payment obligations. Majority of Reece customers maintain trading credit accounts with Reece –– that is, trade supplies are invoiced against their respective trade accounts, with customer given 30 days (inclusive) to pay off their invoices.

Currently our branch staff understand intuitively how likely our customers are to pay their invoices on time through examining transactional information and based on their intuition, initiating conversations with customers who may need to discuss working through payment terms in a given period. However, this exercise is mostly manually administered (through branch staff eyeballing TRS debtor histories) and dependent on branch staff’s experience; Reece is considering providing supporting capabilities to help all branches use data to more systematically identify and prioritise customers to speak to about invoice payments.

### The Data
The DBAs who manage TRS have delivered extracts from 4 tables from the production databases:

- **accounts.csv**: Contains account information for our customers
- **skus.csv**: Contains the details about our product lines
- **invoices.csv**: Contains the invoices issued to each account
- **invoice_line_items.csv**: Contains the details of the SKUs sold on each invoice

The data can be found in the `task_one/data_extracts` folder in this repository.

### Task One: Building an ETL pipeline to support our Applied Data Scientists
You've been working closely with the Applied Data Scientists in the team to understand what features might be predictive for late invoice payment. Now, the scientists have requested that a dataset be produced on a regular basis. As part of your response, please add to the repository the code and documentation that:

- Transforms the raw data into the features required by the scientists
- Tests your ETL job using the CSV extracts provided
- Highlights any intermediate data models you might use to store the data and why
- Highlights any design choices you've made, as well as scaling considerations

Additional details related to the task are provided in the `task_one` folder.

### Task Two: System Design
Having written the ETL job to do the data transformation required, we now need to design the overall system architecture that will allow the Data Team to operationalise the ETL job and maintain it as a long-lifed production system. As part of your response, please add to the repository the documentation that:

- Shows the architecture of a production system that could run your (and similar) ETL jobs, before exposing the resulting datasets to the various consumers.
- Indicates how your architecture would evolve to support near real-time updating of data as the TRS engineering team enables CDC.
- Highlights any key architectural decisions made, and explains them.

Additional details related to the task are provided in the `task_two` folder.
