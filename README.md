# Winning-Space-Race-with-Data-Science
IBM Data Science Professional Certificate Capstone Project
## 📌 What is Capstone Project?
A capstone project is a final multi-phase assignment typically required at the end of a program. It is the most comprehensive demonstration of everything you have learned throughout your program. It can take various forms, including research papers, presentations, or practical work. It serves as a bridge between academic theory and practical application, helping to develop essential skills such as problem-solving, critical thinking, and communication. The term “capstone” comes from architecture—it refers to the top stone placed on a building to complete it.


## 📊 Data Sources
1.  **SpaceX API:** Collected launch data using a custom Python script.
2.  **Web Scraping:** Scraped Falcon 9 launch records from [Wikipedia](https://en.wikipedia.org/wiki/List_of_Falcon_9_and_Falcon_Heavy_launches) using `BeautifulSoup` to complement the API data.

## 🛠️ Installation & Usage
### Prerequisites
*   Python 3.7+
*   `pip`

### Running the Dashboard Locally
1.  Clone the repo:
    ```bash
    git clone https://github.com/hammadqaiser/Winning-Space-Race-with-Data-Science.git
    cd Winning-Space-Race-with-Data-Science
    ```
2.  Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3.  Run the Dash application:
    ```bash
    python src/spacex_dash_app.py
    ```
4.  Open your browser and go to `http://127.0.0.1:8050/`

### Running the Analysis Notebooks
Launch Jupyter Lab or Notebook from the root directory and navigate to the `Jupyter Notebooks/` folder.

## 📈 Methodology
1.  **Data Collection:** Programmatically gathered data from API and HTML.
2.  **Data Wrangling:** Handled missing values, created new features (e.g., `Landing Outcome`), and normalized data.
3.  **EDA:** Used SQL and Pandas to analyze relationships between variables like launch site, orbit type, and payload mass.
4.  **Interactive Maps:** Created Folium maps to visualize launch sites and outcomes.
5.  **Predictive Analysis:** Trained and evaluated multiple classifiers (Logistic Regression, SVM, Decision Tree, KNN) to predict first stage landing success. Optimized hyperparameters using `GridSearchCV`.
6.  **Dashboard:** Built an interactive web application with Plotly Dash to visualize results and make predictions.

## 🎯 Results & Key Findings
*   The best performing model was **Logistic Regression Classifier** with an accuracy of **83.34%**.
*   Key factors influencing successful landing include:
    *   **Payload Mass:** Lighter payloads have a higher success rate.
    *   **Launch Site:** Certain sites have historically higher success rates.
    *   **Orbit Type:** Missions to specific orbits are more conducive to recovery.
*   **Conclusion:** It is possible to predict first stage landing with high accuracy, and SpaceX's reusability strategy is data-driven. [Summarize your presentation's conclusion].

## 🧩 Technologies Used
*   **Programming Language:** Python
*   **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Plotly, Folium, Scikit-learn, BeautifulSoup, Requests
*   **Dashboard:** Plotly Dash
*   **Development:** Jupyter Notebook, Jupyter Lab, VS Code
*   **Version Control:** Git, GitHub

## 📜 License
This project is licensed under the Apache License - see the [LICENSE](LICENSE) file for details.

## 👤 Author
Hammad Qaiser
*   [LinkedIn](https://www.linkedin.com/in/hammadslash/)

## 🙏 Acknowledgments
*   Data provided by SpaceX and Wikipedia.
*   Inspired by the IBM Data Science Professional Certificate on Coursera.
