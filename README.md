# Qatar Stock Exchange Technical Analysis

This project performs technical analysis on Qatar Stock Exchange (QSE) symbols using TradingView indicators and sends email notifications for trading signals.

## Setup

### Configuration

1. **Copy the example configuration file:**
   ```bash
   cp config.example.ini config.ini
   ```

2. **Edit `config.ini` with your credentials:**
   - Add your Gmail email address
   - Add your Gmail app password (not your regular password)
   
   **Note:** For Gmail, you need to use an [App Password](https://support.google.com/accounts/answer/185833) instead of your regular password. Enable 2-factor authentication on your Google account and generate an app password.

3. **Never commit `config.ini` to version control** - it contains sensitive credentials and is already in `.gitignore`.

## Usage

Run the main analysis script:

```bash
python main_QSE.py
```

The script will prompt you to select:
- Analysis type (Monthly/Weekly/Daily/Hourly)
- Recommendation filter (STRONG_BUY/BUY/NEUTRAL/SELL/STRONG_SELL)
- Symbol list to analyze

## Features

- Technical analysis using TradingView indicators
- Multiple timeframe analysis (M/W/D/H)
- Email notifications with Excel attachments
- Database storage of analysis results
- Customizable symbol lists
