# Daraz Chatbot

This project is a chatbot that scrapes smartphone data from the Daraz website, including ratings, prices, specifications, and reviews. The data is stored in a CSV file and used to provide responses based on user queries. The chatbot is built using Flask for the backend and a simple frontend. It has fixed responses for greetings and tokenizes responses to look for keywords like price, rating, above, below, between, etc., to give appropriate responses.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Features](#features)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/daraz-chatbot.git
    cd daraz-chatbot
    ```

2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Start the Flask server:
    ```bash
    python app.py
    ```

2. Open your web browser and navigate to:
    ```
    http://127.0.0.1:5000
    ```

3. Interact with the chatbot via the web interface.

## Project Structure

- `app.py`: The Flask application that serves the chatbot.
- `scraper.py`: Script to scrape smartphone data from Daraz and store it in a CSV file.
- `data/smartphones.csv`: CSV file containing scraped data of smartphones.
- `templates/index.html`: HTML template for the chatbot's frontend.
- `static/style.css`: CSS file for styling the chatbot's frontend.
- `README.md`: This file.

## Features

- **Data Scraping:** Scrapes smartphone data from Daraz, including ratings, prices, specifications, and reviews.
- **Data Storage:** Stores the scraped data in a CSV file for easy access and querying.
- **Chatbot Responses:**
  - Fixed responses for greetings.
  - Keyword-based responses for queries about price, rating, specifications, etc.
- **Flask Backend:** Uses Flask to handle backend logic and serve the chatbot.
- **Simple Frontend:** A user-friendly web interface to interact with the chatbot.

## Examples

Here are some example queries and responses:

**User:** Hi<br>
**Chatbot:** Hello! How can I assist you today?

**User:** Show me smartphones with a rating above 4<br>
**Chatbot:** Here are some smartphones with a rating above 4:
- Smartphone 1: Rating 4.5, Price: $299
- Smartphone 2: Rating 4.2, Price: $399

**User:** What is the price of Smartphone 3?<br>
**Chatbot:** The price of Smartphone 3 is $499.

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue to improve the project.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
