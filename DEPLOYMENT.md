# Deployment Instructions

## Step 1: Push to GitHub

1. **Create a new GitHub repository:**
   - Go to https://github.com/new
   - Repository name: `incrementality-calculator` (or your preferred name)
   - Make it **Public** (required for Streamlit Community Cloud free tier)
   - Don't initialize with README (we already have one)

2. **Connect your local repo to GitHub:**
   ```bash
   git remote add origin https://github.com/YOUR_USERNAME/incrementality-calculator.git
   git push -u origin main
   ```

## Step 2: Deploy to Streamlit Community Cloud

1. **Go to Streamlit Community Cloud:**
   - Visit: https://share.streamlit.io/
   - Sign in with your GitHub account

2. **Create new app:**
   - Click "New app"
   - Select your GitHub repository: `YOUR_USERNAME/incrementality-calculator`
   - Branch: `main`
   - Main file path: `app.py`
   - App URL: Choose a custom URL (e.g., `incrementality-calculator`)

3. **Deploy:**
   - Click "Deploy!"
   - Streamlit will automatically install dependencies from `requirements.txt`
   - Your app will be available at: `https://YOUR_APP_NAME.streamlit.app/`

## Step 3: Verify Deployment

1. **Check the app loads correctly**
2. **Test with sample inputs:**
   - Channel: YouTube
   - Monthly Spend: $10,000
   - Cost per Form: $600
   - Test Duration: 8 weeks
   - MDE: 20%, Power: 80%, P-Value: 0.05

3. **Expected result should show:**
   - Statistical parameters (power/p-value) now impact results
   - Budget cap toggle working (enable/disable, adjustable multiplier)
   - Clean formatting without broken asterisks
   - Proper indication when results are capped vs uncapped

## Troubleshooting

**If deployment fails:**
- Check the deployment logs in Streamlit Community Cloud
- Verify all imports work correctly
- Ensure requirements.txt has correct versions

**If the app runs but has errors:**
- Check for any missing imports
- Verify all file paths are correct
- Test locally if possible with: `streamlit run app.py`

## App Features

✅ **Working Features:**
- Statistical parameters (MDE, Power, P-Value) properly impact calculations
- Configurable budget cap toggle (enable/disable, adjustable 1.5x-20x)
- CPA properly impacts calculations
- Cross-channel interaction disclaimers and proper sourcing
- Multiple confidence level scenarios
- Clean formatting and professional UI
- Transparency when results are capped vs uncapped

✅ **Ready for Production Use**