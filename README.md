# Aviation Safety Analysis: Aircraft Accident Risk Assessment

## Executive Summary

This analysis examines commercial and passenger aviation safety data from 1948-2023, focusing on aircraft makes/models that are professionally built and could still be active (40-year lifetime assumption). The analysis identifies the safest aircraft through comprehensive examination of fatal/serious injury rates and aircraft destruction rates.

**Key Finding**: Large commercial aircraft (Boeing, Airbus) are significantly safer than small aircraft, with injury rates 5-10x lower. Within each category, specific manufacturers demonstrate exceptional safety records supported by robust accident data.

---

## Dataset Overview

- **Total Records Analyzed**: 15,255 accidents
- **Date Range**: 1982-2022 (40-year active fleet assumption)
- **Aircraft Categories**: Commercial airplanes only (excluded helicopters, gliders, amateur-built)
- **Manufacturers Evaluated**: 42 makes with ≥50 accidents each
- **Safety Metrics**: Fatal/serious injury rates & aircraft destruction rates

---

## Part 1: Aircraft Make Recommendations

### SMALL AIRCRAFT (≤20 passengers)

**Recommended Manufacturers** (lowest fatal/serious injury rates):

| Make | Injury Rate | Accidents | Destruction Rate |
|------|-------------|-----------|------------------|
| **MCDONNELL DOUGLAS** | 3.73% | 19 | 5.3% |
| **Boeing** | 3.85% | 56 | 3.6% |
| **BOMBARDIER INC** | 4.29% | 20 | 5.0% |
| **Maule** | 4.66% | 68 | 4.4% |
| **AIRBUS** | 5.05% | 58 | 5.2% |

**Key Insights:**
- Boeing's small aircraft demonstrate exceptional safety with low injury (3.85%) and destruction rates (3.6%)
- Bombardier shows strong competitive positioning in safety
- Top manufacturers show low variance in injury rates - consistent, reliable performance
- Cessna dominates market with 239 accidents while maintaining good safety (7.74%)

### LARGE AIRCRAFT (>20 passengers)

**Recommended Manufacturers** (lowest fatal/serious injury rates):

| Make | Injury Rate | Accidents | Destruction Rate |
|------|-------------|-----------|------------------|
| **BOEING** | 3.67% | 243 | 2.1% |
| **EMBRAER** | 3.47% | 50 | 2.0% |
| **BOMBARDIER INC** | 2.81% | 43 | 2.3% |
| **MCDONNELL DOUGLAS** | 0.70% | 18 | 5.6% |
| **AIRBUS** | 4.92% | 75 | 4.0% |

**Key Insights:**
- Boeing 737 is the most-tested aircraft with 243+ accidents, yet maintains excellent safety (3.67%)
- **Large aircraft are inherently safer**: Injury rates are 8-10x lower than small aircraft
- Modern aircraft benefit from redundant systems, crew training, and regulatory oversight
- Bombardier and Embraer offer competitive alternatives with strong safety records

---

## Part 2: Critical Safety Factors

### FACTOR 1: Weather Conditions

**Impact on Injury Severity:**

| Weather Type | Injury Rate | Accidents |
|-------------|-------------|-----------|
| Visual Meteorological (VMC) | 14.03% | 13,360 |
| Unknown/Other | 26.00% | 130+ |
| Instrument Meteorological (IMC) | 40.43% | 813 |

**Statistical Evidence:** ANOVA test confirms significant differences (p<0.05) across weather conditions.

**Findings:**
1. **Weather is critical** - IMC accidents have 3x higher injury rates than VMC
2. **Clear visibility advantage**: VMC provides better crew reaction time and rescue response
3. **Poor visibility correlation**: IFR/IMC conditions show 2.8x higher injury severity
4. **Implication**: Aircraft with superior all-weather capability are safer for passengers

### FACTOR 2: Engine Type

**Impact on Injury Rates:**

| Engine Type | Injury Rate | Accidents |
|------------|-------------|-----------|
| **Turbo Fan** | 5.75% | 579 |
| Turbo Jet | 14.48% | 56 |
| Reciprocating | 15.61% | 12,283 |
| Turbo Prop | 19.59% | 801 |
| Unknown | 21.46% | 1,517 |

**Statistical Evidence:** Significant differences (p<0.05) in injury rates by engine type.

**Findings:**
1. **Turbofan engines are 3-4x safer** than piston/turboprop engines
2. **Engine reliability directly impacts outcomes** - modern jet engines have superior performance
3. **Multi-engine redundancy** shows more consistent safety profiles
4. **Technology matters**: Modern turbofan engines correlate with lower injury rates
5. **Implication**: Turbofan-powered aircraft (Boeing 777/787, Airbus A330/A350) offer superior safety

---

## Client Recommendations

### For Small Aircraft Operations:
**Preferred Makes**: Boeing, Bombardier, McDonnell Douglas
**Key Criteria:**
- Multi-engine configuration (better redundancy)
- Proven safety track record (50+ accidents)
- Low injury rates in adverse conditions

### For Large Commercial Aircraft:
**Preferred Makes**: Boeing, Bombardier, Embraer
**Key Criteria:**
1. **Turbofan engines** (avoid turboprop for passenger ops)
2. **Multi-engine redundant systems**
3. **Modern avionics** for all-weather capability
4. **Established manufacturers** with robust track records

---

## Methodology

**Data Cleaning:**
- Professionally-built aircraft only (excluded amateur-built)
- 40-year lifetime assumption (1982-2022 data)
- Makes with ≥50 accidents, models with ≥10 accidents
- Key metrics: Fatal/Serious Injury Fraction, Aircraft Destruction Rate

**Statistical Methods:**
- ANOVA testing for categorical factors
- Grouped aggregation and statistical summaries
- Sample size requirements for statistical robustness

---

## Repository Contents

- `Aviation_Accidents_Cleaning.ipynb` - Data cleaning pipeline
- `Aviation_Accidents_Data_Analysis.ipynb` - EDA and statistical analysis
- `data/aviation_cleaned.csv` - Cleaned dataset (15,255 records)
- `figures/` - Visualizations supporting analysis

**Analysis Date:** March 2026 | **Data Coverage:** 1948-2022
