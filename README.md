IBM Z Datathon

Team name: **Malatang**

Team members: 
- Thanesphol Leerungruang
- Cheng-Ching Lei
- Seungyeon Yang
- Ka Yu Wong
- Elena Lickel

**Machine Learning Model for Predicting Housing Prices in England and Wales**

**Abstract**

This project addresses the challenge of accurately predicting housing prices in England and Wales, with a specific focus on the impact of local infrastructure and amenities, including transport links. Leveraging a decade of historical housing price data from the Office for National Statistics (ONS) and incorporating proximity to critical amenities such as tube stations, parks, and community facilities, we developed a robust linear regression model and utilized XGBoost regression. This model aids in understanding and forecasting the dynamics of housing prices, providing insights that are crucial for policymakers, investors, and urban planners. By utilizing IBM Z for secure and high-performance processing, our solution ensures efficient handling of large datasets and real-time analytics, fostering equitable growth and transparency in the housing market. Our work contributes directly to Sustainable Development Goal 11, promoting inclusive, safe, and sustainable urban environments. 

**Problem Statement**

The housing market in England and Wales encapsulates a complex ecosystem influenced by multifarious socio-economic factors, where infrastructure—particularly transport links—plays a pivotal role in determining property values. An accurate and reliable predictive model that can systematically evaluate the influence of such amenities on housing prices is not just a technological advancement but a necessity for achieving equitable growth in urban and rural areas alike.
This initiative aligns closely with the Sustainable Development Goals (SDGs), particularly SDG 11, which aims to make cities and human settlements inclusive, safe, resilient, and sustainable. By understanding and predicting housing price trends, stakeholders from government bodies to individual homeowners can make better-informed decisions, thus fostering communities that are economically viable and socially inclusive.

**Data Utilization**

For our predictive model, we utilized an extensive dataset sourced from the Office for National Statistics (ONS), which provides detailed insights into housing prices in England and Wales over the past decade. This dataset includes quarterly housing price data, allowing for nuanced analysis of trends over time. The core components of our dataset are as follows:

- Price Data: Historical housing prices adjusted for inflation to ensure accuracy in trend analysis. This adjustment helps in understanding the real growth or decline in property values, independent of general economic inflation.

- Location Data: This includes the proximity to critical infrastructure like tube stations, which is a significant factor in property valuation. Proximity to essential services can dramatically influence the desirability and hence the price of properties.

In a subsequent stage of our analysis, we extended our dataset to include various amenities provided by each area, which plays a crucial role in assessing the true value of properties. Amenities include, but are not limited to:

- Access to Amenities: Detailed information about the accessibility to tube stations, ATMs, community facilities, libraries, parks, play areas, post offices, and rail stations. These amenities were recorded in separate files such as 'accesstoamenitiesatms.xlsx', 'accesstoamenitiescommunityfacilities.xlsx', etc., providing a comprehensive view of what each neighborhood offers.

- Travel Time to Amenities: Understanding the travel time to critical infrastructures like rail stations further enhances the dataset's granularity, allowing us to factor in convenience as a pricing variable.

By analyzing these elements, our model can identify outliers indicating whether properties are overpriced or underpriced relative to the amenities they offer. This outlier analysis is crucial for stakeholders interested in finding undervalued properties or in understanding areas that might be overvalued.

The rich dataset from the ONS combined with our detailed amenity data allows for a robust analysis, providing stakeholders with actionable insights that go beyond simple price predictions to understand the underlying factors driving market dynamics. This approach not only aids in making informed investment decisions but also in policy-making and urban planning, ensuring sustainable development in alignment with community needs and infrastructure growth.


**Model Development:**

Initial Approach: The project began with a linear regression model to establish a baseline understanding of the factors affecting housing prices.
Advanced Techniques:
XGBoost: To address non-linear relationships and improve predictive accuracy, we integrated the XGBoost algorithm, renowned for its performance in regression tasks.
Clustering: We applied clustering techniques to categorize regions by similar characteristics, identifying areas that are potentially underpriced or overpriced.
