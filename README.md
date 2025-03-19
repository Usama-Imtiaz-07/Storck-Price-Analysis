# **S&P 500 Stock Price Analysis Web App**

## **Project Overview**
This project is a **Streamlit-based web application** that provides real-time insights into the **S&P 500** stock market. The app retrieves the list of S&P 500 companies from **Wikipedia** and fetches their **year-to-date stock closing prices** using the **yfinance** library. Users can filter companies by sector, visualize stock price trends, and download the data for further analysis.

---

## **Features**
1. **S&P 500 Company List**:
   - Displays the list of S&P 500 companies with details such as **symbol**, **name**, **sector**, and **sub-industry**.
   - Allows users to filter companies by **sector** using a sidebar multiselect dropdown.

2. **Stock Price Visualization**:
   - Fetches and displays **year-to-date closing prices** for selected companies using **yfinance**.
   - Generates interactive line charts to visualize stock price trends.

3. **Data Download**:
   - Enables users to download the filtered S&P 500 data as a **CSV file** for offline analysis.

---

## **How It Works**
1. **Data Retrieval**:
   - The app scrapes the S&P 500 company list from **Wikipedia** using `pandas.read_html`.
   - Stock price data is fetched in real-time using the **yfinance** library.

2. **User Interaction**:
   - Users can select specific **sectors** to filter companies.
   - A slider allows users to choose the number of companies (1 to 5) for which stock price charts are displayed.

3. **Visualization**:
   - The app uses **Matplotlib** to plot the closing prices of selected stocks.
   - Charts are displayed directly in the app for easy interpretation.

---

## **Technologies Used**
- **Python Libraries**: Streamlit, Pandas, yfinance, Matplotlib, Seaborn, NumPy, base64.
- **Data Source**: [Wikipedia](https://en.wikipedia.org/wiki/List_of_S%26P_500_companies).
- **Deployment**: Streamlit (web-based).

---

## **How to Run the App**
1. **Install Dependencies**:
   ```bash
   pip install streamlit pandas yfinance matplotlib seaborn numpy
   ```

2. **Run the App**:
   ```bash
   streamlit run app.py
   ```

3. **Access the App**:
   - Open the provided URL in your browser to interact with the app.

---

## **Screenshots**
1. **S&P 500 Company List**:
   ![Company List](screenshots/company_list.png)

2. **Stock Price Visualization**:
   ![Stock Price Chart](screenshots/stock_price_chart.png)

3. **Data Download**:
   ![Download CSV](screenshots/download_csv.png)

---

## **Future Enhancements**
- Add more interactive features like **technical indicators** (e.g., moving averages, RSI).
- Enable comparison of multiple stocks on the same chart.
- Integrate **machine learning models** for stock price prediction.

---

## **Contributors**
- Usama Imtiaz
