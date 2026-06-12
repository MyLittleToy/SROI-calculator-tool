# Interactive SROI (Social Return on Investment) Calculator

A lightweight, browser-based web application designed for non-profits and charities to quantify their social and economic impact credibly. 

###The Problem
Calculating Social Return on Investment (SROI) traditionally requires complex, fragile Excel models. Non-profit teams often struggle with the tedious math of applying compound impact discounts (deadweight, attribution, displacement, and annual drop-off) across multi-year cycles. This tool streamlines the data modelling process into a transparent, interactive pipeline.

## Key Features
* **Dynamic Impact Discounting:** Automatically applies standard SROI filters (Deadweight, Attribution, and Displacement) to raw outcome data.
* **Multi-Year Financial Modelling:** Compounds annual drop-off rates across an evaluation period of up to 30 years.
* **Net Present Value (NPV) Pipeline:** Integrates a standard financial discount rate to calculate the true present value of future social benefits.
* **Instant Stakeholder Reporting:** Outputs a clear, headline impact ratio (e.g., £3.50 of social value created for every £1 invested) designed for funders and trustees.

## Tech Stack & Development Process
* **Frontend:** Single-file HTML5, CSS3 (responsive design), and Vanilla JavaScript for the calculation engine.
* **Development Methodology:** Built using an AI-assisted workflow. I acted as the Product Manager and Architect—designing the financial logic, defining the mathematical formulas for the discount compounding, and iteratively prompt-engineering a Gen AI assistant to write and debug the functional code.

## How to Use This Tool
Because the application is built entirely using standard web technologies, there is no setup required:
1. Clone this repository or download the `index.html` file.
2. Double-click the file to open it instantly in any modern web browser.
