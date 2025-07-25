<<<<<<< HEAD
# Incrementality-Experiment-App
Estimate incrementality for different experiments

A practical Streamlit application for calculating budget requirements for marketing incrementality testing.

## Features

- **Industry-Standard Multipliers**: Uses 1.5-5x budget multipliers based on actual incrementality testing practices
- **CPA Integration**: Properly factors in Cost Per Acquisition to determine required budgets
- **Statistical Parameters**: Adjusts for Minimum Detectable Effect, Statistical Power, and P-Value thresholds
- **Cross-Channel Awareness**: Includes disclaimers and context about cross-channel interactions
- **Multiple Scenarios**: Pre-configured confidence levels for easy comparison

## Important Limitations

This calculator provides simplified budget estimates for single-channel incrementality testing. It does NOT account for:
- Cross-channel interactions (YouTube → Search → Conversion)
- Media mix synergies (10-35% of effectiveness per academic research)
- Attribution overlap between channels
- Organic lift from paid campaigns

For comprehensive incrementality measurement, consider Media Mix Modeling or multi-touch attribution solutions.

## Usage

1. Select your marketing channel (YouTube, Facebook, Google Search, etc.)
2. Input current monthly spend and cost per form
3. Set test duration and form-to-AQL conversion rate
4. Adjust statistical parameters (MDE, Power, P-Value)
5. Review budget requirements and feasibility assessment

## Sources & Methodology

Based on industry practices from:
- Google Ads conversion lift studies (Geographic holdout testing)
- Meta Business conversion lift (User-level RCTs)
- Academic research: Naik & Raman (2003) on cross-media synergies
- Marketing Science Institute (2019) cross-channel attribution research

## Deployment

This app is designed to run on Streamlit Community Cloud. Simply connect to a GitHub repository and deploy.

## Requirements

- Python 3.8+
- Streamlit 1.28.0+
- pandas, scipy, numpy
