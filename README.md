This paper presents a comprehensive life cycle assessment of "Foodforecast," a machine learning service that helps German bakeries reduce food waste through better demand forecasting. Here are the key points relevant to your bakery waste reduction project:

## Core Findings

**Impact on Waste Reduction:**
- The ML system achieved an average 30% reduction in bakery returns across 175 bakeries in 2022
- Prevented approximately 2,000 tons of food waste annually
- Reduced return rates from around 19.6% to 16.9%
- Bread and rolls showed the largest absolute reduction in waste

**Environmental Benefits:**
- The environmental benefits of avoiding food waste outweighed the system's computing impacts by 1-3 orders of magnitude
- This held true across multiple impact categories (carbon emissions, resource depletion, energy demand, and water eutrophication)
- Even when considering different end-of-life scenarios for bakery returns (composting, energy recovery, donation), the net environmental benefit remained strongly positive

## Technical Implementation

**How the System Works:**
- Uses recurrent neural networks (RNN) to analyze historical sales data
- Considers external factors like weather, holidays, and local events
- Generates daily demand-adjusted forecasts for each product and store
- Integrates with existing bakery ERP systems

**Key ML Operations:**
- Data processing and inference dominated computational requirements (together ~95% of ML compute)
- Model training was surprisingly minor (~3-6% of compute)
- The system trains individual models for each bakery to capture location-specific patterns

## Practical Insights for Your Project

1. **Focus on Accuracy Over Efficiency**: The paper shows that improving forecast accuracy yields far greater environmental benefits than optimizing computational efficiency

2. **Product Clustering**: Group bakery products into categories based on similar characteristics (ingredients, shelf life, production process) for more effective modeling

3. **Infrastructure Considerations**: Cloud-based solutions proved more efficient than on-premises computing due to better resource utilization

4. **Baseline Challenges**: Establishing accurate baseline waste levels is crucial but challenging - consider both historical data and parallel testing approaches

5. **Trade-offs to Consider**: While reducing waste is beneficial, be aware that overly conservative forecasts could lead to stockouts and lost sales

This research strongly validates the potential of AI-based demand forecasting for reducing bakery waste, demonstrating that the environmental benefits substantially outweigh the computational costs of running such systems.
