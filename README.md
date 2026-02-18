# cheese_forecasting_data_model
Excel‑based data model for a UK cheese importer to forecast profit and loss under different Euro–Pound exchange rates and economic conditions.

The model helps non‑technical users see how changes in exchange rates, margins and sales volumes will affect total profit, using calculations, scenario analysis and clear charts.

2. Key features
Home page user interface with buttons that navigate to all key sheets (Base Sheet, Prediction Sheet, Charts), making it easy for users to move around the model.
​Base Sheet for entering core business data such as cheese type, cost per kilo in Euros, monthly sales, and calculated profits at a given exchange rate.
Prediction Sheet that adjusts sales and profits based on changes in the Euro–Pound exchange rate and an increment value, showing how profit changes under different scenarios.
Graphic Chart sheet that compares profit per cheese type (and total profit) between the base scenario and the prediction scenario, giving a quick visual view of risk and opportunity.
Input and output fields clearly defined with data types, validations, formatting rules and example values, so the model can be understood and extended by other users.
​

3. Technical details
Tooling: Microsoft Excel.
​Core functions used:
Absolute cell referencing for exchange rate and margin fields (for example, using cells like B12 B12 and B13 B13 as fixed parameters).
IF functions to adjust monthly sales based on changes in exchange rate increments.
​
Calculated fields for:
Cost in GBP = cost per kilo in Euros × exchange rate.
Profit margin = cost in GBP × margin percentage.
Selling price in GBP = cost in GBP + profit margin.
Profit in GBP = (selling price – cost in GBP) × monthly sales.

Data model structure:
Input fields: Cheese name, cost per kilo in Euros, monthly sales volume, exchange rate, margin.
Output fields: Cost in GBP, selling price in GBP, profit margin, profit per cheese, total profit.

4. Business logic and scenario
Business context:
The company imports cheeses (e.g., Camembert, Emmental, Gruyere, Edam, Gouda) in Euros and sells them in GBP.
When economic growth is strong, sales and prices are higher; when growth is weak, sales fall and profit drops.
​

Scenario modelling:
Users adjust:
Exchange rate (e.g., 0.7 Euro → GBP)
Increment value (e.g., 0.1), which simulates changes in economic or market conditions.
The Prediction Sheet uses these inputs to:
Reduce or increase monthly sales volumes.
Recalculate profit per cheese.
Recalculate total profit for the company.

5. How to use the workbook
Open Data-Model-Assingment-2.xlsx in Excel.
​Start on the Home Page sheet and use the buttons to navigate to:
Base Sheet – view and edit the base data.
Prediction Sheet – view scenario results.
Graphic Chart – view charts comparing profits.

On the Base Sheet:
Enter or adjust:Cheese type, Cost per kilo in Euros, Monthly sales volumes, Check that exchange rate and margin values are correct.

On the Prediction Sheet:
Change the Increment and Exchange Rate to simulate different scenarios.
Review the updated profit per cheese and total profit.

On the Graphic Chart sheet:
Use the chart to visually compare base vs prediction profits for each cheese and for the total.
​

6. Skills demonstrated
This project demonstrates: Spreadsheet‑based data modelling for a real‑world business scenario.
Scenario and “what‑if” analysis using Excel formulas and parameters (exchange rate, increment, margin).
Clear input/output design, including field descriptions, validation rules and formatting.
​Building a simple user interface in Excel with a home page and navigation buttons.
​Communicating model design through documentation and slides (storyboards, flow diagram, test plan).
