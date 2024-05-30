# Fuel Price Notification

## Description
This Python project, named `fuel_price_notification.py`, is hosted on PythonAnywhere and performs daily tasks to notify users about fuel prices when they are at cyclic lows in Adelaide. It leverages emerging AI technologies through the OpenAI API to condense a buying tip from the ACCC. The price is calculated as the 5th percentile value for all prices in Adelaide for any specific fuel type. Notifications are sent using the Pushover API to users who provide a user key.

## Features
- **Daily Fuel Price Updates**: Monitors and notifies about cyclic lows in fuel prices.
- **AI-Enhanced Insights**: Uses OpenAI's API to generate concise and actionable fuel buying tips.
- **User Notifications**: Sends alerts through the Pushover API based on user preferences.

## Dependencies
- `datetime`
- `pytz`
- `sys`
- `requests`
- `bs4`
- `openai`
- `boto3`
- `numpy`
- `statistics`
- `config` (Custom configuration module)

## Setup
1. Clone the repository and navigate to the project directory.
2. Install required Python packages:
- pip install datetime pytz requests beautifulsoup4 openai boto3 numpy statistics
3. Ensure you have the necessary API keys and credentials configured in the `config.py` file:
- OpenAI API Key
- Pushover Application Token
- AWS Access Keys for DynamoDB interactions
- FPDAPI Subscriber Token for fetching fuel prices

## Usage
Run the script as a standalone and independent tool
