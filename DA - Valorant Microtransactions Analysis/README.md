# In-game Purchases Analysis

### Project Objectives
The aim of this project is to derive insights through purchases from the game Valorant. 
- Purchases in this game offer only aesthetic value and not any advantages.
- The scope of this project will be limited to consumer behaviour as data is not exhaustive and conditional on making at least one purchase within the game. 

To avoid biases, we gather insights that are not affected by this condition.
Some common business metrics such as average revenue per user (ARPU), lifetime value (LTV) and conversion rates would inevitably be skewed, thus omitted in the scope of this project. 

Proxying users' activity to purchase history was briefly considered as it would shed light on trends in important metrics such as daily/monthly active users (DAU/MAU), retention/churn rate, but was ultimately deemed too far-fetched due to the presence of too many unknown factors.

### Dataset
The dataset consist of transactions from over 110 unique players that was gathered through goodwill and publicly available sources.
Conversion to in-game currency was done through Excel's vlookup based on the amount spent and the conversion based on their region/country's in-game store. 
For a small amount of transactions (0.77%) where conversion can't be done, it is approximated with its closest points bundle.

### Proxies/Assumptions
Proxies or assumptions taken:
- Time of purchase of in-game currency is accompanied with a subsequent purchase in the game itself during the same session.


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
- Due to the nature of data collection, most popular bundles are not conclusive.
- Relatively safe to assume which are the least popular bundles based on dataset.


### Recommendations
Sales
- If the goal is to maximise revenue, there may be a potential to engage in more aggressive pricing for smaller points packages.
- However, it is important to note that the action should be aligned with the overall company's strategic direction and image.

Battle/Season Pass
- If sales are inferior to competitors and distribution (10 to 15%) are significantly different, incentives or rewards can be adjusted accordingly to consumers' behaviour to entice and drive an increase in sales.

Weapon Bundles
- Similarities between features and art of least popular bundles can be identified and subsequently avoided, to prevent poor sales of future bundles if relevant. 
- However, I believe the purpose of having such bundles are to juxtapose the difference in qualities and to further increase the appeal for a premium/hyped bundle that is being planned for future release.
- If the previous point is true, stagger good bundles from new season dates as average order value (AOV) suggest a somewhat price-sensitive audience and a simultaneous purchase of a battle pass and a weapon bundle may reduce the ARPU.

