# China Cross-Border E-Commerce Growth and Operations Dashboard
A data analytics portfolio case study project analyzing 7001 rows of a China cross-border e-commerce enterprise sales data from 2019 to 2025. 

## Executive Summary

This case study dives into the development of an interactive growth and operations dashboard analyzing ¥88.4M in cross-border transaction volume across 139,193 annual orders.

Through a multi-dimensional segmentation, the analysis revealed that 41% (¥45M) of the total annual revenue was driven by high-value customers where funnels were optimized by targeted app push campaigns. Conversely, a bottleneck was spotted in the “at-risk customer” segment where a significant checkout drop off was observed which directly correlates to a grueling 19-20.5 hours of customer service response time. 

To repair this leaky revenue pipeline and promote high-value loyalty, the dashboard provides stakeholders with the cross-filtering clarity in reworking the system by: 

1. Shifting the marketing budget into segment-specific channel allocations;
2. Transitioning from discount-based retention to value-based loyalty;
3. Deploying automated chatbot workflows; and
4. Optimizing logistics routes and incorporating an order’s real-time location updates.

## Business Problem

The cross-border e-commerce company is currently facing a Jevons paradox. While the company is currently acquiring customers, four critical operational and strategic bottlenecks are eroding profitability and threatening long-term retention:
1. **Inefficient customer acquisition:** The current one-size-fits-all marketing strategy across different acquisition channels is driving up customer acquisition cost (CAC) while delivering low conversions.
2. **Discount-driven customer behavior:** Customers, particularly the price-sensitive, cost-conscious, and at-risk customer segments, have conditioned themselves to only make the purchase decision when a voucher is available. Thus, rendering the company’s revenue model to be dependent on price incentives.
3.	**Fragmented and slow customer support:** With customers interacting across five distinct channels, the support infrastructure is struggling to maintain service levels where response times ballooned to a grueling 19-20.5 hours, creating a poor customer experience.
4.	**Logistics friction:** As a cross-border entity, the company faces inherent challenges which the current data suggests are exacerbating customer dissatisfaction. 

## Data Acquisition and Preparation

The initial dataset, acquired from Kagggle.com, presented significant barriers to analysis due to critical inconsistencies in text and temporal data. Key challenges included unnecessary underscores and erratic capitalization that obscured content readability, alongside a high-risk ambiguity in the date column where “dd/mm/yyyy” and “mm/dd/yyyy” formats were used interchangeably. Resolving these issues was essential to ensure data integrity, as failing to standardize the text and unify the chronological timeline would have rendered any subsequent trend analysis fundamentally flawed. 

To address these data quality issues, I implemented a series of targeted Excel transformations to standardize the dataset:

*	**Text Cleaning:** Applied the SUBSTITUTE function to remove all extraneous underscores, replacing them with spaces to restore natural word delimiters.
*	**Case Standardization:** Constructed a custom formula using PROPER, LOWER, MID, and LEFT functions to convert inconsistent text into uniform sentence case.
*	**Date Harmonization:** Leveraged TEXT parsing functions to detect and convert mixed “dd/mm/yyyy” and “mm/dd/yyyy” entries into a single, consistent “dd-mm-yyyy” format.
* **Category Refinement:** Replaced the non-standard “55_Above” label with “55+” to ensure age bracket consistency and improve readability.

## Methodology and Analysis

To address the company challenges, I transformed the raw data into a functional management tool where the dashboard’s interface was engineered using a user-centric UI/UX framework rather than a random assembly of charts. The architectural objective was to minimize cognitive load for stakeholders, allowing them to move from macro-organizational health to micro-operational root causes in less than three clicks.

The structural canvas was broken down into a strategic 3-Zone Layout Hierarchy:

* **Zone 1 – Financial and Customer Value:** Occupying the entire left side of the dashboard, this column serves as the structural baseline. It houses the high-impact KPI cards and the macro customer trends (i.e., Purchase Per Generation (Sum), and Customer Value Longevity). The logic here ensures that an executive’s natural “F-shaped” reading pattern immediately registers core financial performance before diving into operational data.
*	**Zone 2 – Marketing and Funnel Performance:** Positioned in the center of the canvas, this zone transitions the viewer from high-level financial outcomes into customer intent and action (i.e., User Experience Conversion Funnel, Acquisition Channels, and Customer Discount Dependency). This zone answers the vital question, “What user paths and promotional habits are driving those numbers?”
*	**Zone 3 – Operations, Logistics, and Customer Support:** Placed intentionally as the final destination in the left-to-right reading flow. This zone functions as the diagnostic wing of the infrastructure, monitoring shipping friction, hub performance, and customer support metrics.

While the filters were intentionally chosen to give users instantaneous granular control over the entire dashboard:

*	**Target Customer:** This slicer was selected because aggregate data often lies by averaging out completely different groups of people. This enables the stakeholders to have a power to isolate “High-value” from “At-risk” or “Price-Sensitive” cohorts and to transform static charts into a targetable marketing tool.
*	**Preferred Language:** This is chosen specifically to bridge global marketing adjustments with operational support. Because cross-border e-commerce relies heavily on localized communication, cross-referencing language preferences with conversion drops or customer service response rates allows teams to quickly deploy localized fixes (e.g., transactional updates or language-specific support reps).
*	**Transaction Year:** This is essential for establishing historical trajectory. In cross-border e-commerce, macro environments shift rapidly due to global trade policies; adding a temporal filter allows leadership to separate short-term operational anomalies and long-term systemic trends.

## Data Insights

By analyzing the data through a segmented lens rather than looking only at global averages, the dashboard uncovers critical operational gaps and clear revenue opportunities across different customer groups. The following deep-dives turn these interactive data views into direct, strategic recommendations to protect business margins and improve cross-border logistics.

<img width="927" height="321" alt="Baseline" src="https://github.com/user-attachments/assets/12f30c9d-c293-4934-a3c8-6965bae32646" />

#### A.	The Baseline Benchmark

The business operates at a healthy volume with ¥88.4M in total annual spend and ¥686 in average order value (AOV) across 139,193 annual orders, with customers putting in more money starting 2022 up to 2025 from its downfall in 2021. The primary audience of the enterprise are surprisingly young within the age bracket of 25-34, followed by 35-44, and then 18-24. 

The general user experience conversion funnel revealed the effectivity of the marketing campaigns, mainly by affiliate channels and app push campaigns, driving 793,356 page views every month, with 205,575 monthly cart additions. However, there was a significant checkout drop-off converting only 139,193 orders annually. 

The significant checkout drop-off can be explained mainly by shipping friction which has an average delay of 2.23 days in United States, and 2.19 days in Russia and Brazil where the top three most orders come from despite Shandong and Fujian hubs does their absolute best. This means that while demand is high overseas, international customs and long-haul shipping modes are major bottlenecks compared to near-region shipping to Spain or Singapore. Another factor contributory to this checkout drop-off number is customer satisfaction which correlates to customer service response time.

<img width="929" height="322" alt="High-value customer segment" src="https://github.com/user-attachments/assets/e5a56490-17be-4f4d-9805-9a1107abca5d" />

#### B.	High-Value Customer Segment

When filtering for high value customers, performance metrics drastically shifted: AOV surged by 27% to ¥870 from ¥686. This segment alone brought in more than half of the company’s total revenue (¥45M), despite making only about 41% (57,145) of the total orders. 

Interestingly, these customers were acquired mainly through app push campaigns. This means that they have already downloaded the platform’s app in their mobiles phones and that they are engaged, repeat-buyers responding to direct and personalized mobile alerts. Also, these customers are noted to complete their purchases with or without being bribed with discount vouchers.

Another important insight in this customer segment is the relative customer satisfaction (89.5% to 90.5%) across customer support functions when their concerns are entertained within 10.6 to 11.2 hours of customer service response time, although mediocre when compared to industry leaders. When addressing their concerns, this customer segment is highly satisfied with the performance of chatbot, then email support and phone support, and followed by live agent. In terms of hub performance, Shandong, Beijing, and Fujian hubs performs at their best, incorporating the shipping friction in their efficiency. 

<img width="928" height="321" alt="At-risk customer segment" src="https://github.com/user-attachments/assets/67e18f2c-6fb3-49cd-ae33-edf37ac139b7" />

#### C.	At-Risk Customer Segment

Enabling the at-risk customer filter, notable insights can be acquired even when looking at the performance metrics alone. This customer segment brought in 3,129 annual total orders converting ¥1.7M in annual revenue. What’s notable is the 23% (¥847) increase in AOV compared to the baseline ((¥686). 

This customer segment is dominated by 25–34-year-olds who may have less disposable income which means they are after the best value for their money. Following are the 35–44-year-olds who are at the peak of their careers and have more disposable income but wants convenience, and then the 18–24-year-olds who are still forming their brand preferences. This suggests that with a small improvement in service, the customers in this segment may be converted into loyal, buying customers.

While looking at the marketing and funnel performance, a broken funnel immediately catches one’s eyes. Out of 40,883 monthly page views, there are only 4,626 monthly cart additions. Worse, a catastrophic drop off before the checkout is observed resulting in only 3,129 total orders annually, that is roughly 261 orders only per month. The reason for this is a grueling 19 to 20.5 hours of customer service response time across all channels. Because the customers are forced to wait nearly a full day before their concerns is addressed, they abandon their carts leaving a very low customer satisfaction score of only 48 to 50%.

#### D.	Price-Sensitive Customer Segment

When the filter for price-sensitive customers was selected, a significantly compressed AOV of ¥546, a 20% decline from the company baseline, can be observed. But this brought in ¥6.1M in total spend across 13,611 orders. 

Interestingly, this customer segment’s conversion behavior is reliant on social discovery, such as social media and marketplace banners, and they are highly correlated to high discount values with 0.70+ index rating. Their funnel shows 132,203 monthly page views but drops to only 19,752 monthly cart addition. These customers spend a significant amount of their time window-shopping and scrolling through social feeds, only pulling the trigger when there is a steep promotional code applicable at checkout.

<img width="928" height="322" alt="Price-sensitive cutomer segment" src="https://github.com/user-attachments/assets/92e7742f-f7ab-449b-94e0-a13e68fd0ad2" />

## Conclusion and Strategic Recommendations

Through the development of this interactive dashboard, critical bottlenecks in the customer journey have been brough into focus. Regardless of the customer segment, the data confirms that marketing inefficiencies, customer discount dependency, slow customer support cycles, and shipping delays are systemic issues impacting high-value customers, loyalty-oriented customers, cost-conscious customers, price-sensitive customers, and at-risk customers alike. Nonetheless, the visibility gained from these insights transform these challenges from ambiguous problems into actionable opportunities for immediate operational improvement.

To address these systemic issues, the following strategic actions are recommended:

* **High Marketing Cost and Low Conversion:** Instead of being okay with the current one-size-fits-all marketing strategy, the company should shift into segment-specific channel allocation. This means doubling down on the top performing acquisition channels for each customer segment, and cutting on what doesn’t work. The enterprise may follow this budget allocation structure: 70-20-10. Allocate 70% of marketing budget on proven winners. While spend 20% on optimizations such as A/B testing of ad copies and ad creatives. Then allot the 10% on experiments such as mediocre acquisition channels but only if they meet a strict ROI threshold for 30 days. Finally, immediately pause or cut ad spend on channels that consistently show higher CAC than lifetime values (LTV).
* **Customer Discount Dependency:** The enterprise should think of ways to transition from discount-based retention to value-based loyalty. Essentially, this is just providing more value, with no incremental cost incurred to the company, to every customer segment. An example of this is creating a loyalty program that rewards at-risk customers with free shipping or early access instead of a 20%-off voucher. Another example is A/B testing non-monetary incentives for high-value customers to see if they convert without any single discount code.
* **Slow Customer Support Cycles:** Instead of whishing that customer service response channels would be able to handle every customer concern smoothly, the enterprise may consider looking into its operation for areas that need optimization. It can implement an AI-powered triage system and optimize staffing schedules. That means, routing simple queries (e.g., tracking, return, product details, shipping time) exclusively to the chatbot with improved NLP, reducing staff load by approximately 40%. In addition, the company may create and utilize a time-series data by scheduling customer service response staffs during peak inquiry windows to cut average response time from 20 hours to 4 hours. Training the customer service response staffs frequently on addressing different customer concerns can also help bring the average response time down to 4 hours.
* **Shipping Delays:** The company may provide both a tangible and a psychological solution to this problem. The tangible solution is to optimize logistics routing. They can negotiate alternative carriers for the specific regions with 2-3 delay days. They can also establish regional warehouses in the US to fulfil orders in the local and neighboring states and countries. While the psychological solution to this, is to update their website by displaying a dynamic, region-specific delivery estimates, rather than a generic “5-7 day estimated arrival.” They can also add a dynamic image showing the current location of the customer’s orders and the specific points it needs go through. These strategies reduce the “Where is my order?” support tickets.

By implementing these data-driven strategies, the enterprise can anticipate 20-30% reduction in marketing waste by focusing on already-wining acquisition channels, increased customer LTV by breaking the cycle of discount dependency, and a 40-50% improvement in customer satisfaction score by reducing customer support response time, and minimizing order delays. 

The dashboard serves as a real-time monitoring tool to track the success of these recommendations. Future iterations should include performance vs. target view to measure the ROI of these initiatives.


---

 ## Tools and Concepts Used
* **Microsoft Excel:** Data cleaning and standardization, data modeling, pivot tables, dynamic slicers and dashboard
* **Data Visualization:** Executive KPI cards along with other financial and customer values, marketing and funnel performance, and operation, logisics, and customer support.

## How to View the Project
* **For the Dashoard:** Download the "China Cross-Border E-Commerce CRM Dataset.xlsx" file above to test the interactive slicers
* **For the Case Study Discussions:** Click the "Portfolio Project - China Cross-Border E-Commerce Growht and Operations Dashboard.pdf" above to read about the bottlenecks and the recommended actions in solving the company's systemic issues.
