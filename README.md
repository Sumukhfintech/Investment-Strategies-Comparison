# 📊 Investment Portfolio Comparison

This project evaluates and optimizes various investment portfolios using Python, with a focus on analyzing the **risk-return trade-offs** of different asset allocation strategies. Designed for a **risk-averse investor**, the analysis considers **mean-variance efficiency**, historical data, and portfolio composition through comprehensive visualization and performance metrics.

---

## 📁 Portfolios Compared

- **All-Equity Portfolio**
- **Traditional 60/40 Portfolio (60% Equities / 40% Bonds)**
- **Harry Browne’s Permanent Portfolio (seasoninv in the code)**
- **Ray Dalio’s All Seasons Portfolio (rayinv in the code)**
- **Custom Portfolio: 45% in the market, 25% in Baa Corporate Bonds, 30% in Real Estate**

---

## 🎯 Objective

To determine the most suitable portfolio strategy for a risk-averse investor based on:
- Historical risk/return characteristics
- Portfolio volatility
- Diversification benefits
- Mean-variance efficiency (current, 1930s, 1980s, 2010s)

---

## 📈 Asset Classes & Their Roles

| Asset Class              | Pros                                                                 | Cons                                                                 | Role in Portfolio                                                    |
|--------------------------|----------------------------------------------------------------------|----------------------------------------------------------------------|----------------------------------------------------------------------|
| **S&P 500 (Equities)**   | - High potential long-term returns<br>- Capital gains & dividends    | - High volatility<br>- Sensitive to economic changes                 | Growth engine; suitable for long-term investment                    |
| **T-Bills**              | - Near risk-free<br>- Highly liquid                                  | - Low returns                                                        | Safety net in downturns; cash-like stability                        |
| **T-Bonds**              | - Lower volatility than equities<br>- Steady interest income         | - Sensitive to interest rate changes<br>- Lower returns than stocks | Income generation with lower risk                                   |
| **Baa Corporate Bonds**  | - Higher yields than government bonds<br>- Fixed income source       | - Higher default risk<br>- Interest rate sensitivity                | Moderate-risk income; diversifies bond exposure                     |
| **Real Estate (REITs)**  | - Potential price appreciation<br>- Low correlation with stocks      | - Illiquid<br>- Cyclical performance                                | Inflation hedge; diversification benefit                            |
| **Gold**                 | - Hedge against inflation & crises<br>- Store of value               | - No income generation<br>- Storage/insurance costs                 | Defensive asset; performs well in volatile markets                  |

![image](https://github.com/user-attachments/assets/4b7eb16e-6b1e-460a-9372-e4e0548ec275)

Asset classes on the efficient frontier

![image](https://github.com/user-attachments/assets/71e8a6c5-058c-4e6c-b3c7-ad4b1f72babb)

Returns of different assets over time

---
## 📈 The portfolios and their pros & cons

| Portfolio                        | Pros                                                                 | Cons                                                                                                                   |
|----------------------------------|----------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------|
| **Custom portfolio**             | - This portfolio has lower standard deviation than S&P 500, indicating less volatility. <br>- It also indicates less extreme minimum return, which may imply lower drawdowns.                 | -This portfolio has a lower mean return compared to S&P 500, suggesting less growth potential.<br>- The maximum return is also lower than the S&P 500, indicating less upside. |
| **S&P 500**                      | - S&P500 has highest mean return, which indicates strong growth potential. <br>- S&P500 has highest maximum return, suggesting high potential for large gains.                                | Equities have the highest standard deviation, indicating greater volatility and risk.<br>- S&P500 has the most negative minimum return, signifying potential for significant loss. |
| **60/40 portfolio**              | - This portfolio has moderate mean return, balancing risk and reward. <br>- The portfolio ha ower standard deviation than S&P 500, suggesting more stability.                                 | - The portfolio has lower mean return than the S&P 500, implying less growth.<br>- The minimum return here indicates potential for notable losses, though not as extreme as S&P 500. |
| **Brown's portfolio**            | - This portfolio has the lowest standard deviation, implying the least volatility among the portfolios.<br>- The portfolio has moderate maximum return, indicating some growth potential.     | - This portfolio has the lowest mean return, which might not satisfy growth-oriented investors.<br>- Minimum return suggests the possibility of losses, although less than more volatile portfolios. |
| **Ray Dalio's 60/40 portfolio**  | - Ray Dalio’s portfolio has a good balance for mean return and standard deviation, indicating a moderate risk/reward profile.<br>- Maximum return is reasonable, showing potential for gains. | - Ray Dalio’s portfolio has slightly higher standard deviation compared to bostoninv and seasoninv, which might indicate more risk.<br>-The lower mean return than the S&P 500, suggesting less potential for growth. |

---

## Metrics and mean-efficient frontiers

## 📊 Portfolio Performance Metrics

| Metric          | Custom (bostoninv) | S&P 500 | Traditional 60/40 (tradinv) | All Seasons (seasoninv) | Permanent (rayinv) |
|-----------------|--------------------|---------|------------------------------|--------------------------|--------------------|
| **Sharpe Ratio**     | 0.492             | 0.427   | 0.461                        | 0.451                    | 0.491              |
| **VaR 95%**          | -0.098            | -0.228  | -0.134                       | -0.037                   | -0.046             |
| **Beta**            | 0.475             | 0.940   | 0.560                        | 0.207                    | 0.274              |
| **Treynor Ratio**   | 0.105             | 0.089   | 0.101                        | 0.159                    | 0.134              |

## KDE of portfolios & Assets

![image](https://github.com/user-attachments/assets/af8239db-00cc-48e8-a074-7ad02b16b49d)

## Current Efficient frontier of all portfolios

![image](https://github.com/user-attachments/assets/65c18c75-c983-4b2e-8f59-0ea9560f8221)

![image](https://github.com/user-attachments/assets/9fe27bed-6ac3-40d9-b61b-23349b12a9fe)

1. Through the 1930s, a time where the all equity and traditional portfolio became popular just before the Great Depression were not mean-variant effcient. This is because of the volatility during the great depression.

![image](https://github.com/user-attachments/assets/ea9ce91e-5017-49ac-bd0d-21e85122acf4)


2.Seasonal portfolio which was introduced during the 1980s was mean-variant efficient. This might be because of the overall boom in the US economy.

![image](https://github.com/user-attachments/assets/c3d779c1-6b52-4361-95f9-ec3ccaab98aa)


3. Ray Dalio's investment portfolio introduced during the 2010s is mean-variant efficient. This can be because of the lob-sided recovery post the great recession. (It is highly weighted in T-Bonds which had high yields and were a safe bet post-2008. Our custom portfolio is also mean-variant efficient because of the real-estate recovery post-2008.

![image](https://github.com/user-attachments/assets/6fad9355-2c43-4bc3-b16b-fe7dc45b938a)

---

## Conclusions & Limitations

From this study, we can fiund that S&P 500 gives the best return and is also mean-variance efficient. Additionaly, we also found that there are other portfolios that are mean-variance efficient and has better Sharpe Ratio and requires further study to conduct indepth analysis. Our custom portfolio has the highest Sharpe ratio among other portfolios (0.492364), which means that slightly better returns for the level of risk involved than all others. It has comparatively smaller Beta of 0.474730, which means that the portfolio is less sensitive to market movements. In addition, the proposed portfolio has very low potential downside risk value (VaR) of 0.09847. Moreover, it lies on the mean-variance frontier, which indicates that it has an optimal combination of risk and return. 
Hence, we can state that our portfolio can be a good starting point for a risk-averse investor. 

We are doing analysis on yearly data which does not fully capture price movements. We do not have much information about the investors preferences which will impact the study. The study also does not consider transactional cost and taxes.

---

