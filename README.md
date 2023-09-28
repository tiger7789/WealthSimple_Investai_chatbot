# 🤖️InvestAI Chatbot🤖️

Welcome to the InvestAI Chatbot, a smarter way to manage your investments and financial aspirations. Explore various scenarios and make well-informed choices that align with your financial goals.

## Table of Contents

1. [Functions Import](#functions-import)
2. [Sample Portfolios](#sample-portfolios)
3. [Scenario 1: Creating an Account](#scenario-1-creating-an-account)
4. [Scenario 2: Risk Profile](#scenario-2-risk-profile)
5. [Scenario 3: Investment Updates](#scenario-3-investment-updates)
6. [Scenario 4: ETFs Recommendation](#scenario-4-etfs-recommendation)
7. [Integration of Codes](#integration-of-codes)

---

### Functions Import <a name="functions-import"></a>

This section of the code involves importing the necessary functions and libraries that the InvestAI Chatbot relies on.

```python
# Setting up the environment and importing all the functions
!pip install numpy-financial
from numpy_financial import rate
from sklearn.preprocessing import MinMaxScaler
from sklearn.neighbors import NearestNeighbors

import yfinance as yf
import matplotlib.pyplot as plt
import pandas as pd
import seaborn as sns

# Set a professional theme for plots
sns.set_style("whitegrid")
```
---
### Scenario 1: Creating an Account <a name="scenario-1-creating-an-account"></a>

**Explanation:** In this scenario, the InvestAI Chatbot helps users create an account based on their investment goals and demographic information. It begins by gathering essential customer information, such as their first name, age, residency status, and annual income. The chatbot then validates the user's eligibility for various investment options based on this information. If the user meets the criteria, they are presented with a list of investment goals to choose from, such as building an emergency fund, buying a home, achieving financial independence, saving for retirement, or improving credit score.

### Scenario 2: Risk Profile <a name="scenario-2-risk-profile"></a>

**Explanation:** In this scenario, the chatbot evaluates the user's risk profile by asking a series of questions and collecting user responses. The questions cover various aspects of risk tolerance, investment time horizon, comfort with fluctuations in investment value, familiarity with investment options, and reactions to market volatility. Based on the user's responses, the chatbot calculates a total risk score and categorizes the user's risk tolerance. The risk categories typically range from "Extreme Low" to "High."

### Scenario 3: Investment Updates <a name="scenario-3-investment-updates"></a>

**Explanation:** In this scenario, the chatbot provides users with the ability to receive updates on their investments. Users are prompted to provide their username and password, which allows the chatbot to access their investment portfolios. The chatbot then presents the available portfolios associated with the provided credentials. Users can select a specific portfolio and choose a timeframe to review its performance. Additionally, users have the option to compare their selected portfolio with other Exchange-Traded Funds (ETFs) to gain insights into investment trends.

### Scenario 4: ETFs Recommendation <a name="scenario-4-etfs-recommendation"></a>

**Explanation:** In this scenario, the chatbot assists users in making informed decisions about investing in Exchange-Traded Funds (ETFs). The chatbot leverages the user's risk profile from Scenario 2 to recommend suitable ETFs that align with the user's risk tolerance and financial goals. It calculates the user's required rate of return based on their investment horizon, initial investment amount, and desired future value. Using this required rate of return and the user's risk ranking, the chatbot filters a list of ETFs. It recommends ETFs that match or exceed the user's required rate of return and are within their risk tolerance. Users can then explore these recommended ETFs and their historical performance to make informed decisions about diversifying their investment portfolios and optimizing their strategies.
