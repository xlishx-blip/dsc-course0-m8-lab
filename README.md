# Aviation Accident Analysis

# Project overview
This project was completed for an airline and airplane insurance client seeking guidance on aircraft safety. Using aviation accident records from 1983–2023 (filtered to exclude retired makes/models beyond a 40 year lifetime), the analysis identifies which aircraft makes and specific models have the lowest rates of total destruction and the lowest likelihood of serious or fatal passenger injuries in the event of an accident
Separate recommendations are provided for small aircraft (≤20 passengers) and large aircraft (≥20 passengers). All comparisons are restricted to makes/models with a minimum of 10 recorded incidents to ensure statistical robustness

# Dataset
Source: Aviation accident records, 1948–2023 (filtered to 1983 onwards)
Columns used:
  - serious_and_fatal_fraction — proportion of passengers seriously or fatally injured per incident
  - aircraft_destroyed — binary indicator of total aircraft loss
  - make, model_make — manufacturer and specific model
  - total_passengers — used to split small vs. large aircraft
  - weather_condition — VMC, IMC and UNK
  - number_of_engines 

# Key Findings

- Large aircraft significantly outperform small aircraft on a per-accident basis. The best large-aircraft makes achieve near 0% injury fractions and 0% destruction rates 
- Small aircraft injury rates are higher that large aircrafts across top makes, suggesting make choice matters but no single make is safer than another in this category.
- Weather condition is a strong influence of accident outcome. IMC and UNK weather conditions result in aircraft destruction above 50% of the time and lower rates are linked to VMC
- Engine count with single and 2 engine aircraft show high median injury fractionscompared to aircraft with 3 or more engines show considerably lower median outcomes,however is goes back to high median at 8 engines. Eveb if the engine is linked to destruction its not the ideal factor to look at.

# Recommendations:

## Small Aircraft

Recommended Makes:
Makes considered safest: 
- Waco
- Grumman-Schweizer
- Helio 
- Maule

Waco and Grumman-Schweizer lead on passenger safety. All small-aircraft recommendations carry the caveat that per-accident risk is inherently higher than large aircraft across the board.

Recommended Specific Models:
- Bell 47D-1 
- Grumman G164B
- Cessna 180C 
- Diamond Aircraft DA 20 C1
- Maule MX-7-235

## Large Aircraft

Recommended Makes:
- Aero Commander
- Gulfstream
- Sikorsky 
- Dehavilland 
- Swearingen

Aero Commander, Gulfstream, Sikorsky, Dehavilland and Swearingen are the top-tier recommendations, achieving 0% on both metrics. Lockheed and Douglas are the aircrafts with highest risk despite appearing in the top 15.

Recommended Specific Models:
- Boeing 717-200
- Boeing 757-232 
- McDonnell Douglas MD-88 
- Boeing 757-222
- Embraer EMB-145LR 

Boeing 757 variants appear multiple times across the top tier, indicating safe model. The Boeing 717-200 is the single strongest model recommendation for large aircraft due to its low rates of destruction.

# Conclusion
According to the 15 selected makes, larger planes are linked to less severe outcome of injury and destruction compared to smaller planes.
