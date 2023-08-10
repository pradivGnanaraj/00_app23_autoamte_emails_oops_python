# Email News Sender

This Python script sends personalized news updates to a list of recipients based on their interests. It fetches news articles using the News API and sends them via email using the Yagmail library.

## Features

- Fetches news articles based on user interests using the News API.
- Sends personalized emails containing news articles to recipients.
- Supports scheduled email sending based on time.

## Getting Started

1. Install the required dependencies by running:

   ```
   pip install -r requirements.txt
   ```

2. Add your News API key and Gmail credentials to the respective places in the code.

3. Prepare the `people.xlsx` file with recipient information, including `name`, `email`, and `interest`.

4. Run the script using:

   ```
   python main.py
   ```

   The script will send personalized emails containing news articles to recipients at the specified time.

## Configuration

- **News API:** Obtain an API key from [News API](https://newsapi.org/) and replace `"INSERT YOUR API KEY HERE"` in `news.py` with your API key.

- **Gmail Credentials:** Replace `"YOUR GMAIL ADDRESS"` and `"PASSWORD OF YOUR GMAIL ADDRESS"` in `main.py` with your Gmail credentials.

## File Descriptions

- `main.py`: The main script that reads recipient information from `people.xlsx`, fetches news articles, and sends emails.
- `news.py`: Contains the `NewsFeed` class that interacts with the News API to fetch news articles.
- `people.xlsx`: Excel file containing recipient information.
- `requirements.txt`: List of required Python libraries.

## Usage

1. Define recipient information in `people.xlsx`.
2. Run the script using `python main.py`.
3. The script will send personalized news emails to recipients at the specified time.

## Credits

- [Yagmail](https://yagmail.readthedocs.io/en/latest/) - Library for sending emails using Gmail.
- [News API](https://newsapi.org/) - Provides access to a wide range of news articles.

## License

This project is licensed under the [MIT License](LICENSE).

---
