# In-game Purchases Analysis

### Project Objectives
This analysis seeks to derive insights into consumer behaviour using purchases in the game Valorant. Purchases in this game offer only aesthetic value and not any advantages.

The scope of this project will be limited to identifying consumer behaviour within transactions as data is not exhaustive and conditional on making at least one purchase within the game. 

To avoid biases, we gather insights that are not affected by this condition.
Some common business metrics such as average revenue per user (ARPU), lifetime value (LTV) and conversion rates would inevitably be skewed, thus omitted in the scope of this project. 

Proxying users' activity to purchase history was briefly considered as it would shed light on trends in important metrics such as daily/monthly active users (DAU/MAU), retention/churn rate, but was ultimately deemed too far-fetched due to the presence of too many unknown factors.

### Dataset
Game sales data have and always will be safely guarded information. The dataset consist of transaction data from over 110 unique players that was gathered through goodwill and publicly available sources.
Conversion to in-game currency was done through Excel's vlookup based on the amount spent and the conversion based on their region/country's in-game store.

### Proxies/Assumptions
Proxies or assumptions taken:
- Time of purchase of in-game currency is accompanied with a subsequent purchase in the game itself.


### Takeaways
Sales Analysis
- Approximately 80% of recorded transactions fall under the equivalent of US$40 which suggests a relative price-sensitive audience.
- Approximately 40% of total transactions are multiple purchases in the same session. This could be a result of:
	1. Including different points packages to reach a specific amount of desired points
	2. Weapon bundle CTA with displayed discount led to additional purchase (for entire bundle)
	3. Consumers overcame initial purchase inertia, thus increasing willingness-to-pay

Battle/Season Pass Analysis
- In comparison to a proportional average of a 90-day period of 1.12%, in this case 2 days of 2.24%:
	- Sales from the first two days of the battle pass launched comprised of 14.12% of total transactions in its 90 days period.
	- Number of transactions from the first two days of the battle pass launched comprised of 11.33% of total transactions in its 90 days period. 

Weapon Bundles Analysis
- Due to nature of data collection, most popular bundles are not conclusive.
- Relatively safe to assume which are the least popular bundles based on dataset.


### Recommendations
Sales
- If the goal is to maximise revenue, there may be a potential to engage in more aggressive pricing for smaller points packages.

Battle/Season Pass
- If sales are inferior to competitors and distribution (10 to 15%) are significantly different, incentives or rewards can be adjusted accordingly to consumers' behaviour to entice and drive an increase in sales.

Weapon Bundles
- Similarities between features and art of least popular bundles can be compared to avoid poor sales of future bundles if relevant. However, I believe the purpose of launching such bundles are used to juxtapose the difference in qualities and further increase the appeal for a 'good/hyped' bundle that is being planned to release in the future.
- If the previous point true, stagger good bundles from new season dates as average order value (AOV) suggest a somewhat price-sensitive audience and a simultaneous purchase of a battle pass and a weapon bundle may reduce the ARPU.

