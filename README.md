# Gravity Model
Date: 06/11/2024


# Introduction
The Gravity Model of Trade is a widely used framework in international economics that explains trade flows between countries based on their economic size and geographical distance. This assignment explores the application of the gravity model to analyze trade patterns among nations, incorporating key factors such as distance, GDP, shared borders, language, and OECD membership. Using empirical data from 2005, the analysis examines the relationships between trade volume and these variables, highlighting their statistical significance and economic implications.

This study evaluates the extent to which economic size and geographical proximity influence trade by utilizing regression analysis and visual representations such as scatter plots. The findings reveal a negative correlation between trade volume and distance, confirming that higher transportation costs and logistical barriers reduce trade. Conversely, a strong positive relationship is observed between trade and combined GDP, aligning with the economic theory that larger economies engage in greater trade. Additionally, factors such as shared borders, common language, and historical colonial ties significantly contribute to increased trade flows.

This study also investigates the impact of OECD membership on trade, assessing whether membership in this economic organization facilitates trade between member nations. The results indicate that while OECD membership aligns policies and reduces trade barriers, it does not necessarily lead to higher trade volumes among members, suggesting the presence of other influencing factors.

Through this analysis, this project  provides valuable insights into the determinants of international trade, reinforcing the relevance of the gravity model in understanding global trade patterns.


## Descriptive Statistics

![image](https://github.com/user-attachments/assets/3b6739d2-e383-4236-a51e-bae869de588d)


## Scatter Plot for Trade and Distance

![Trade_and_Distance_scatter_plot](https://github.com/user-attachments/assets/17e3434e-52a9-4a65-83f2-d4c17fc4dbfb)

From Figure 1 above, the trend line has a slight downward slope, indicating a negative correlation between Log(Trade) and Log(Distance). This implies that as the distance between trading partners increases, the trade volume tends to decrease, though the relationship is not extremely strong. 
In trade economics, distance is often considered a proxy for transportation costs and other trade barriers. A greater distance between countries usually implies higher transportation costs, logistical challenges, and potentially less frequent trade. Therefore, we would generally expect a negative relationship, as observed in this plot, between distance and trade volume.


## Scatter Plot for log Trade and Log Combined GDP

![Trade_and_combinedGDP_scatter_plot](https://github.com/user-attachments/assets/e0b2c8c3-6759-4e46-ac70-d1e0613c5d8a)

The trend line has a noticeable upward slope, indicating a positive correlation between Log (Trade) and Log (Combined GDP). This suggests that as the combined GDP of two trading partners increases, the trade volume between them also tends to increase.
In international trade theory, GDP is often used as an indicator of economic size and potential market capacity. Larger combined GDP implies that both countries have greater economic output, consumption capacity, and potentially more resources to engage in trade. Therefore, a positive relationship between combined GDP and trade volume aligns with economic expectations.


## Scatter Plot of Trade and Distance, Clustering by Continuity

![Trade_and_Distance_Contiguity_scatter_plot](https://github.com/user-attachments/assets/c08234da-1698-4893-b0e6-966b110af375)

This scatter plot in figure 3 examines the relationship between trade (Log (Trade)) and distance (Log (Distance)), with observations separated by whether or not the trading partners share a common border (contiguity). In this plot:

    Red points (with a red trend line) represent trading pairs that do not share a border (contiguity = 0).
    Blue points (with a blue trend line) represent trading pairs that do share a border (contiguity = 1).
      
The red trend line, representing non-contiguous pairs, has a slightly negative slope. This is consistent with the expectation that greater distance generally reduces trade volume between countries without a shared border, as longer distances likely increase transportation costs and logistical barriers.
The blue trend line, representing contiguous pairs, shows a slight positive slope. This could suggest that, for neighboring countries, an increase in distance does not significantly deter trade. Factors like cultural similarities, established transportation links, and cross-border economic integration may mitigate the negative impact of distance on trade. In fact, longer distances between neighboring countries might still involve trade due to close economic and political relationships.


## Scatter plot for Trade and Combined GDP Clustering by Continuity

![Trade_and_combinedGDP_Contiguity_scatter_plot](https://github.com/user-attachments/assets/35dfa7ba-1a19-422a-80bb-a9a693caf106)

There is a positive relationship between Log (Combined GDP) and Log (Trade) in both groups. As the combined GDP of two countries increases, their trade volume also tends to increase.
The lines representing the trend (fitted lines) for each contiguity level indicate that countries sharing a border (contig = 1) generally have higher trade volumes than those that do not (contig = 0) for similar values of combined GDP.
The trend line for contiguous countries (blue) has a steeper slope compared to the non-contiguous countries (red). This suggests that an increase in combined GDP results in a greater increase in trade for contiguous countries than for non-contiguous ones.
There is more variation in trade volume among non-contiguous country pairs at similar combined GDP levels compared to contiguous ones.


## Scatter Plot for Trade and Distance Clustering by Common Language

![Trade_and_Distance_OffLan_scatter_plot](https://github.com/user-attachments/assets/5f51dfd5-580e-4528-a96b-bdbdc272771a)

Both groups (sharing and not sharing an official language) display a negative correlation between Log (Distance) and Log (Trade). This suggests that as the distance between two countries increases, the volume of trade between them generally decreases.
The lines representing the trend for each language-sharing status indicate that countries sharing an official language (blue line) have higher trade volumes than those that do not (red line) at similar distance levels. This reflects that sharing a common language likely facilitates trade by reducing communication barriers and enhancing ease of business.
The trend line for countries that do not share an official language has a steeper downward slope compared to those that do. This suggests that distance has a slightly stronger negative effect on trade volume for country pairs without a common official language, possibly because the lack of a shared language exacerbates the barriers created by physical distance.


## Scatter plot of Trade and combined GDP by Common Language

![Trade_and_CombinedGDP_OffLan_scatter_plot](https://github.com/user-attachments/assets/4d13c94b-dc08-456d-811e-54e5a4fad4a5)

There is a positive relationship between Log (Combined GDP) and Trade for both groups, suggesting that as the combined GDP of two countries increases, trade volume between them also increases.
The trend lines show that countries sharing a common official language (blue line) generally have higher trade volumes than those that do not (red line) for a given level of combined GDP. This implies that sharing an official language is associated with higher trade volumes, likely due to reduced communication barriers and smoother transaction processes.
The slope of the trend line for countries sharing a common language is steeper than for those that do not. This suggests that as combined GDP grows, the increase in trade volume is more pronounced for countries with a shared language. This might indicate that language plays a role in amplifying the economic potential for trade.


# Correlation Matrix

![Screenshot (277)](https://github.com/user-attachments/assets/c146ad40-1c68-4cab-9ff6-9d6389a797ca)

Log (Trade) and Log (Distance): The correlation coefficient is −0.152860, indicating a weak negative correlation. This suggests that as the distance between countries increases, trade volume tends to decrease slightly. However, the effect is not very strong, implying that distance alone may not significantly influence trade.
Log (Trade) and Log (Combined GDP): The correlation coefficient is 0.648363, which indicates a moderate to strong positive correlation. This suggests that as the combined GDP of two countries increases, trade volume also increases. This relationship is expected, as countries with larger combined economic sizes generally have higher trade volumes.
The matrix suggests that trade volume is more closely related to combined GDP than to distance, with distance having a weak negative impact on trade and combined GDP having a strong positive impact. This aligns with economic intuition that larger economies trade more, and while distance may affect trade, it does not outweigh the influence of economic size.


# Regression Results for Trade for SE model and RSE model

![image](https://github.com/user-attachments/assets/d28aaa7d-9357-4189-b8f3-2c92d7bd87e9)

Adjusted R-squared: The adjusted R-squared is 0.5944, which suggests that the model does not suffer significantly from overfitting and that most variables are likely contributing meaningfully to explaining trade. F-Test: The F-statistic is 476.4886 with a significance level of p < 0.01. This high F-statistic indicates that the model is statistically significant, meaning that the independent variables, taken together, significantly explain the variation in trade volumes.

The coefficient for Log (Distance) is -0.7973, and it is statistically significant (p < 0.01). This negative coefficient indicates that distance has a strong inverse relationship with trade volume, as expected in gravity models. Specifically, a 1% increase in the distance between two countries is associated with approximately a 0.8% decrease in trade. This result aligns with economic theory, as increased distance generally increases transportation costs, reduces ease of access, and can hinder the development of trade relationships.

## Relevance of Additional Factors for Trade Partners

**Common Border (Contiguity)**

The coefficient for Contiguity is 0.3968 and is statistically significant at the 5% level (p < 0.05). This positive coefficient indicates that countries sharing a border trade about 39.7% more than countries that do not share a border, all else being equal. This finding aligns with expectations, as neighboring countries benefit from reduced transportation costs, easier logistics, and often stronger cultural and economic ties, which encourage trade.

**Common Language (Official)**

The coefficient for Common Language (Official) is 1.0867, statistically significant at the 1% level (p < 0.01). This large positive coefficient suggests that sharing an official language has a strong impact on trade, with countries that share a common official language trading approximately 108.7% more than those that do not. This result highlights the importance of linguistic commonality in facilitating communication, reducing misunderstandings, and enhancing trust, which are crucial for international trade relationships.

 **Colonial Relationship**

The coefficient for Colony is 0.6567, also statistically significant at the 1% level (p < 0.01). This positive coefficient suggests that countries with a historical colonial relationship trade approximately 65.7% more than those without such a relationship. The colonial relationship may foster long-lasting institutional, legal, and economic ties that persist beyond the colonial period, thus facilitating trade.


# The effect of GDP on trade, for both importers and exporter’s GDP

The coefficients for Log (Imports) (importer’s GDP) and Log (Exports) (exporter’s GDP) are 0.7343 and 0.7658, respectively, and both are statistically significant at the 1% level (p < 0.01). These positive coefficients indicate that larger economies (with higher GDPs) tend to trade more, which is consistent with the gravity model of trade.

    •	Importer’s GDP (Log (Imports)): The coefficient of 0.7343 suggests that a 1% increase in the importer’s GDP is associated with an approximately 0.73% increase in trade volume. This relationship is likely due to the fact that countries with higher GDPs have greater consumption capacity, enabling them to import more goods and services.
    •	Exporter’s GDP (Log (Exports)): The coefficient of 0.7658 suggests that a 1% increase in the exporter’s GDP is associated with an approximately 0.77% increase in trade volume. Higher GDP in the exporting country generally means more production capacity and a greater ability to export goods and services.
    
Together, these results indicate that trade volume between two countries is positively influenced by the economic size of both the importing and exporting countries, as larger economies tend to have more resources to both import and export.


# OECD Membership

## Scatter Plot for Trade and Distance by OECD Membership

![Trade_and_Distance_OECD_Pair_Scatter_Plot](https://github.com/user-attachments/assets/867d8c0e-f473-44a0-a46b-dc592cb67097)


**OECD Membership Effect :** The plot suggests that OECD membership is associated with higher trade volumes, regardless of distance, possibly due to harmonized policies, economic alignment, and reduced trade barriers. OECD pairs tend to trade more than non-OECD pairs at similar distances.

**Distance Effect by OECD Membership :** Distance appears to reduce trade more for OECD pairs than for non-OECD pairs, as indicated by the steeper negative slope for OECD pairs. However, OECD membership may lessen the overall impact of distance on trade when compared to non-OECD countries.
This visualization supports the hypothesis that OECD membership positively impacts trade volumes. OECD pairs tend to trade more with each other than non-OECD pairs, potentially due to favorable trade agreements, economic cooperation, and aligned standards among OECD countries. Additionally, while distance affects trade among OECD members, it seems to have a more muted effect among non-OECD countries.


## Regression Results


![image](https://github.com/user-attachments/assets/ecd7c799-cdcc-4817-bcca-44c373768335)


### Effect of Being an OECD Member on Trade
The coefficient for the OECD membership variable is -0.1476 with a p-value significant at the 10% level (indicated by the asterisk *). This coefficient suggests that when both countries in a trading pair are OECD members, the trade volume between them is approximately 14.8% lower than it would be for a comparable non-OECD pair, controlling for other variables in the model.
The negative sign on the coefficient is somewhat unexpected, as OECD membership is generally associated with trade facilitation through policy alignment, common economic standards, and reduced barriers. This result might imply that, despite these benefits, other dynamics variables reduce trade volumes between OECD pairs relative to non-OECD pairs.

### Overall Quality of the Model
R-squared and Adjusted R-squared: The adjusted R-squared is 0.5949, meaning that around 59.5% of the variation in trade volume is explained by the model. This is a reasonable fit for trade data, which often contains unobserved factors that can influence trade flows.
F-test: The F-statistic is 409.4166 with a p-value < 0.01, indicating that the model as a whole is statistically significant. This suggests that the included variables, including OECD membership, contribute meaningfully to explaining trade volume between countries.
Adding the OECD membership variable does not drastically improve the model’s goodness of fit but provides additional insights into the effect of OECD membership on trade.

### Effect of OECD Membership
The negative and significant coefficient for OECD membership suggests that OECD membership does not uniformly increase trade between OECD members. Instead, it indicates a reduction in trade between OECD pairs, potentially due to factors like competition or a preference for trading with non-OECD partners for specific goods and services.
This counterintuitive finding might be due to OECD countries diversifying their trade networks beyond other OECD countries or focusing on value-added, high-standard goods where competition within the OECD limits trade volume. This result suggests that while OECD membership aligns policies, it does not necessarily lead to higher trade among OECD members.


# Model Comparison

![image](https://github.com/user-attachments/assets/439c4248-7867-4f65-96e0-0829b43b2a99)


## Overall Quality of the Model

### Adjusted R-squared
The Adjusted R-squared is 0.76, which accounts for the number of predictors relative to the sample size. The high adjusted R-squared suggests that the model remains effective even when considering the degrees of freedom, reinforcing the strong explanatory power of the model.

### Residual Standard Error
The residual standard error is 1.130, which provides an estimate of the average distance that the observed values fall from the regression line. This value indicates the variability in trade volumes that remains unexplained by the model.

### F-test
The F-statistic is 409.4166 with a p-value < 0.01, indicating that the model as a whole is statistically significant. 


## Effect of Distance on Trade
The coefficient for log(distance) is -1.15 and is statistically significant at the 1% level (p < 0.01). This coefficient implies that a 1% increase in the distance between two countries is associated with approximately a 1.15% decrease in trade volume. This negative relationship aligns with the gravity model's prediction that greater distance acts as a barrier to trade due to higher transportation costs, increased logistical challenges, and potentially weaker trade relations over larger distances.

## Effect of OECD Membership on Trade
The coefficient for OECD_pair is 0.084, which is not statistically significant. This suggests that, after controlling for other factors (such as distance, contiguity, and common language), being an OECD member pair does not have a statistically significant effect on trade volume in this model. This lack of significance could imply that OECD membership alone does not automatically increase trade between OECD countries. Other factors—such as economic characteristics, specific bilateral agreements, or regional trade agreements—may play a larger role in determining trade flows among OECD countries.


## Why Should GDP Variables Be Excluded When Using Importer and Exporter Fixed Effects?

### Redundancy of GDP Variables: 

Including fixed effects for importers and exporters absorbs country-specific characteristics, including GDP, that influence trade. Since GDP reflects a country’s economic size and overall trade potential, these effects are implicitly captured by the fixed effects for each country. Adding GDP as separate variables would create multicollinearity, as GDP’s effect would overlap with the fixed effects.

### Other Variables Captured by Fixed Effects

Importer and exporter fixed effects can capture other stable country characteristics, such as institutional quality, economic structure, or cultural factors, that may affect trade patterns. This makes the fixed-effects model suitable for isolating the effect of variables that vary between country pairs (like distance, contiguity, common language, and OECD membership).

## Compare the results of this model with 4. Do you note (if any) the differences of the estimated parameters? Discuss the effect of the OECD variable between the two models

### Distance: 

The structural model shows a stronger negative impact of distance on trade. This could mean that distance-related costs and logistical challenges have a greater independent effect on trade once GDP effects are controlled through fixed effects.

### Contiguity and Common Language

The contiguity effect is slightly stronger in the structural model, while the common language effect is significantly weaker. This difference suggests that some of the language-related trade facilitation in Model 4 was likely influenced by other country-specific characteristics that the fixed effects now capture.

### OECD Membership 

The change in the OECD_pair coefficient from negative and significant in Model 4 to insignificant in the structural model indicates that the impact of OECD membership on trade is not independently significant after controlling for importer and exporter fixed effects. This implies that any trade-facilitating effects of OECD membership may be captured by other country-level factors, such as economic policies and practices inherent to OECD countries, which are absorbed by the fixed effects.

The structural model, with importer and exporter fixed effects, provides a more refined view of trade determinants by isolating the effects of distance, contiguity, language, and OECD membership from country-specific characteristics.


## Differences in Estimated Parameters:

### Distance (log(dist)):

Structural Model (without OECD): The coefficient for log(distance) is -1.151, significant at the 1% level (p < 0.01). This coefficient indicates a stronger negative effect, where a 1% increase in distance leads to an approximate 1.15% decrease in trade.
Question 4 Model: The coefficient for log(distance) was -0.7973, also significant at the 1% level.
Comparison: The structural model without the OECD dummy shows a stronger negative impact of distance on trade. This suggests that when controlling for unobserved country-specific factors (via fixed effects) and excluding the OECD membership variable, distance becomes an even more significant barrier to trade.

### Contiguity (contig):

Structural Model (without OECD): The coefficient for contig is 0.475, indicating that sharing a border increases trade by approximately 47.5%, and this effect is statistically significant.
Question 4 Model: The coefficient for contig was 0.3968, implying a 39.7% increase in trade for bordering countries.
Comparison: The contiguity effect is slightly larger in the structural model, which might indicate that once we control for fixed effects, the natural geographic proximity (border-sharing) has a more pronounced effect on trade.

### Common Language (comlang_off):

Structural Model (without OECD): The coefficient for common language is 0.32, significant at the 5% level, meaning that countries sharing a common official language experience a 32% increase in trade.
Question 4 Model: The coefficient for common language was 1.0867, indicating a much larger effect, with a 108.7% increase in trade.
Comparison: The impact of sharing a common language is significantly smaller in the structural model. This difference suggests that some of the common language effect in the previous model may have been confounded by country-specific factors that are now captured by fixed effects.

### Effect of Distance Between the Two Models

In the structural model without the OECD dummy, the effect of distance on trade is considerably stronger, with a coefficient of -1.151 compared to -0.7973 in the question 4 model.
More Pronounced Trade Barrier: Distance acts as a stronger trade barrier in the structural model, implying that once we control for unobserved country-specific characteristics (via importer and exporter fixed effects), the logistical and cost-related challenges associated with distance become more apparent.
Influence of Fixed Effects: The fixed effects control for country-specific factors like economic size, infrastructure, and institutional quality, which may otherwise obscure the true effect of distance. By isolating these factors, the structural model suggests that distance is a more significant determinant of trade than previously estimated.

