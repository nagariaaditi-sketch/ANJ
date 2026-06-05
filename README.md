# IPO Intelligence Dashboard (India)

An investment-banking style analytics dashboard designed for investors, chartered accountants, and finance professionals to track and analyze Indian IPOs. The application integrates historical statistics, live market returns, Grey Market Premium (GMP) indicators, machine learning listing predictions, and multi-asset Monte Carlo simulation projections.

## 📂 Required Files for GitHub & Deployment

To deploy this application to GitHub and host it on **Streamlit Community Cloud**, upload the following files:

```
├── app.py                  # Main layout router and sidebar routing
├── data_manager.py         # Live price fetching (yfinance), caching, and data loading
├── ml_models.py            # ML predictor and Monte Carlo simulator
├── components.py           # Metrics widgets, Excel and HTML reporting engines
├── styles.css              # Theme CSS stylesheet
├── requirements.txt         # Library dependencies (Crucial for Streamlit Cloud)
├── run_dashboard.bat       # Windows batch quick-run launcher (Optional but helpful)
├── .gitignore              # Ignores temp files like price cache
├── .streamlit/
│   └── config.toml         # Theme settings forcing dark theme
└── data/
    └── historical_ipos.csv # Seed database (Auto-regenerates if missing)
```

## ⚙️ How to Deploy on Streamlit Community Cloud

1. Push all files to a **GitHub repository** (ensure `requirements.txt` and `.streamlit/config.toml` are included).
2. Go to [share.streamlit.io](https://share.streamlit.io/) and log in using your GitHub account.
3. Click **New App**.
4. Configure the deployment settings:
   - **Repository**: Select your GitHub repo name.
   - **Branch**: Select `main` (or the branch you pushed to).
   - **Main file path**: Enter `app.py`.
5. Click **Deploy**. Streamlit Cloud will read `requirements.txt`, install dependencies, load `.streamlit/config.toml` for the dark theme, and launch your live app!
