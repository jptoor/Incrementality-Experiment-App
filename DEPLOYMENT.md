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
   - Reasonable multipliers (1.5-5x range)
   - Proper budget calculations
   - Clean formatting without broken asterisks

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
- Industry-standard budget multipliers (1.5-5x)
- CPA properly impacts calculations
- Cross-channel interaction disclaimers
- Statistical parameter adjustments
- Multiple confidence level scenarios
- Clean formatting and professional UI

✅ **Ready for Production Use**