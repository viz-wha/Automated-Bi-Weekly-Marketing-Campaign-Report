# Automated Bi-Weekly Marketing Campaign Report

This project automates the process of extracting, processing, visualizing, and reporting marketing campaign data. It generates a bi-weekly report that includes key metrics and visualizations, then emails the report to the marketing team.

## Features
- **Data Extraction**: Fetch data from a SQL database or CSV file.
- **Data Processing**: Clean and analyze marketing data.
- **Visualization**: Generate bar charts for campaign performance.
- **Report Generation**: Create an Excel report with raw data and summary insights.
- **Scheduling**: Automate the process to run every 14 days.
- **Email Notification**: Send reports via email (optional, can be enabled).

## Technologies Used
- Python
- Pandas
- Matplotlib & Seaborn
- SQLAlchemy
- OpenPyXL
- Schedule
- Dotenv (for secure environment variables handling)

## Setup Instructions

### 1. Clone the Repository
```sh
 git clone https://github.com/yourusername/marketing-campaign-automation.git
 cd marketing-campaign-automation
```

### 2. Install Dependencies
```sh
pip install -r requirements.txt
```

### 3. Configure Environment Variables
Create a `.env` file in the root directory and set up your credentials:
```env
DB_CONN_STRING="your_database_connection_string"
SENDER_EMAIL="your_email@example.com"
EMAIL_PASSWORD="your_email_password"
SMTP_SERVER="smtp.gmail.com"
SMTP_PORT=465
RECEIVER_EMAIL="recipient@example.com"
```

### 4. Run the Script
To execute the script manually, run:
```sh
python marketing_campaign_analysis.py
```

To run it automatically every 14 days, use:
```sh
python scheduler.py
```

## Deployment Options
- **Local Execution**: Run the script manually.
- **Cron Job (Linux/Mac)**: Automate execution with:
  ```sh
  0 0 */14 * * /usr/bin/python3 /path/to/marketing_campaign_analysis.py
  ```
- **Windows Task Scheduler**: Set up a scheduled task to run the script.

## Contributions
Feel free to submit issues and pull requests to improve this project.

## License
This project is licensed under the MIT License.

## Star the Repo ⭐
If you found this useful, consider giving the repo a star on GitHub!

