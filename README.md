# Web Scrapping With Flask

This is a web scraper application built using Flask and MongoDB. It scrapes customer reviews and ratings for products from <b>Flipkart.com</b> and stores them in a MongoDB database.

## Prerequisites
To run this application, you need to have the following installed on your system:
- Python (version 3.6 or higher)

## Create Virtual Environment for Dependencies
1. Open a terminal and navigate to the project directory.
2. Install virtualenv using the following command (if it is not already installed):
    ```bash
    pip install virtualenv
    ```
3. Create a new virtual environment using the following command:
    ```bash
    virtualenv env
    ```
4. Activate the virtual environment using the following command:
    - On Windows:
        ```bash
        env\Scripts\activate.bat
        ```
    - On Unix or Linux:
        ```bash
        source env/bin/activate
        ```
## Environment Variable Setup
- Create <b>.env</b> file in root directory.
- Write below variable and provide your MongoDb server connect url.
    ```
    MONGO_CLIENT_URL={Your MongoDb Server URL}
    ```
## How to Run the Application
1. Clone the repository to your local machine.
2. Open the terminal and navigate to the project directory.
3. Install the required dependencies using the following command:
    ```bash
    pip install -r requirements.txt
    ```
4. Start the MongoDB server.
5. Run the Flask application using the following command:
    ```bash
    python app.py
    ```
6. Open a web browser and go to http://localhost:5000/.
7. Enter the name of the product for which you want to scrape reviews and click on the "Search" button.
8. The application will scrape the reviews and ratings for the product from Flipkart.com and store them in a MongoDB database.
9. The reviews will be displayed on the web page.

## Functionality
The application has the following functionality:

- Scrapes customer reviews and ratings for a product from Flipkart.com.
- Stores the reviews and ratings in a MongoDB database.
- Displays the reviews and ratings on a web page.
- You can see logs in <b>scrapper.log</b> file.

## Use Cases
The application can be used for the following purposes:

- To analyze customer sentiment for a product by scraping customer reviews and ratings.
- To monitor customer feedback for a product over time.
- To identify common issues or complaints with a product by analyzing customer reviews.