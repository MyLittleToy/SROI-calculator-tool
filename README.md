# Interactive SROI (Social Return on Investment) Calculator

A lightweight, browser-based web application designed for non-profits and charities to quantify their social and economic impact credibly. 

As the Data & Insights Officer for a youth employability charity, I've seen firsthand how calculating Social Return on Investment (SROI) traditionally relies on complex, fragile Excel models. My team constantly struggled with the task of applying compound impact discounts: deadweight, attribution, displacement, and annual drop-off, across multi-year cycles.

I wanted to build a tool that would not only improve our reporting but also provide me with real assurance in our numbers, with the flexibility to adjust values to meet our charity's specific reporting requirements. This tool streamlines the entire data modelling process into a transparent, interactive pipeline I can trust and adapt.

---

## Key Features
* **Dynamic Impact Discounting:** Automatically applies standard SROI filters (Deadweight, Attribution, and Displacement) to raw outcome data.
* **Multi-Year Financial Modelling:** Compounds annual drop-off rates across an evaluation period of up to 30 years.
* **Net Present Value (NPV) Pipeline:** Integrates a standard financial discount rate to calculate the true present value of future social benefits.
* **Instant Stakeholder Reporting:** Outputs a clear, headline impact ratio (e.g., £3.50 of social value created for every £1 invested) designed for funders and trustees.

---

# Example Youth Work Inputs

To help you understand the tool, below is a list of realistic example values for typical youth work or mentoring programmes:

| Input Field | Example Value | Notes |
|-------------|---------------|-------|
| Total programme cost | £50,000 | Annual cost of youth intervention programme serving 100 young people |
| Number of young people reached | 100 | Direct beneficiaries |
| Value of outcome (per person) | £3,500 | e.g., estimated savings from reduced offending, improved mental health, or increased employability |
| Deadweight (%) | 20% | Percentage of positive change that would have happened anyway |
| Attribution (%) | 30% | How much of the change is due to your intervention work (vs family, school, other services) |
| Displacement (%) | 10% | Risk that benefits for some young people cause negative effects elsewhere |
| Drop-off rate (% per year) | 15% | How quickly the positive impact fades over time (e.g., employability gains reducing annually) |
| Evaluation period (years) | 5 | How long you track outcomes post-intervention |
| Financial discount rate (%) | 3.5% | Standard UK Treasury / social value rate for NPV calculations |

**Expected output:**  
With these inputs, you might see an SROI ratio around **£3.20–£4.50** of social value for every £1 invested.

---

## Tech Stack & Development Process
* **Frontend:** Single-file HTML5, CSS3 (responsive design), and Vanilla JavaScript for the calculation engine.
* **Development Methodology:** Built using an AI-assisted workflow. I designed the financial logic, defining the mathematical formulas for the discount compounding, and iteratively prompt-engineering a Gen AI assistant to write and debug the functional code.

---

## How to Use This Tool
Because the application is built entirely using standard web technologies, there is no setup required:

1. Clone this repository or download the `index.html` file.
2. Double-click the file to open it instantly in any modern web browser.
3. Start adjusting values to match your own charity's reporting needs

---

## Limitations
- Not a substitute for full SROI analysis: Formal SROI methodology requires stakeholder engagement, outcome mapping, and financial proxy research. This tool handles the calculation part — you still need quality input data.
- Linear discounting model only: The calculation assumes a straight-line compound discount formula (Net Value × (1 - Drop-off)^y). Real-world youth work outcomes can be non-linear — a young person's confidence might dip, then recover. The model doesn't capture that complexity.
- No sensitivity analysis on individual outcomes: The Sensitivity Simulator tab only stress-tests global assumptions (deadweight, attribution, etc.), not variations in per-outcome proxies or participant counts. If one outcome is driving your ratio, you can't easily see that.
- Proxy values are on you: The tool links to the Manchester Unit Cost Database, but it doesn't validate or suggest proxies. If you enter £0 or unrealistic values, you'll get misleading ratios. Youth work outcomes like "improved resilience" or "reduced isolation" have no built-in financial proxies.
- Mobile experience is limited. Best used on a laptop or desktop.
- No drill-down on charts

**Contributions welcome.**
