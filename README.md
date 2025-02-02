# IPL Win Predictor

## Overview
The **IPL Win Predictor** is a machine learning-based web application that predicts the probability of a team's victory in an ongoing IPL match. The model is trained on historical IPL match data and uses various match parameters such as score, overs completed, wickets lost, and target runs to make real-time predictions.

## Features
- **Team Selection**: Choose the batting and bowling teams from a predefined list.
- **Match Conditions**: Select the host city and set the target score.
- **Match Progress Input**: Enter the current score, overs completed, and wickets lost.
- **Probability Prediction**: The model predicts the probability of the batting team winning the match.
- **Simple UI**: Developed using Streamlit for a user-friendly experience.

## Tech Stack
- **Python**
- **Streamlit**
- **Pandas**
- **Scikit-Learn**
- **Pickle** (for model persistence)

## Dataset
- The model is trained using IPL match data obtained from Kaggle or other publicly available cricket datasets.
- Preprocessing is done using Pandas, and feature engineering includes variables like **current run rate (CRR), required run rate (RRR), balls left, wickets left, and target runs**.

## Installation & Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/Rohansoni45/IPL-Win-Predictor.git
   cd ipl-win-predictor
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Run the application:
   ```sh
   streamlit run app.py
   ```

## Usage
1. Open the Streamlit app.
2. Select teams, city, and enter match details.
3. Click the "Predict Probability" button to get real-time win predictions.

## Model Details
- The model is a **Logistic Regression classifier** trained on past IPL match data.
- Features used:
  - Batting Team
  - Bowling Team
  - Host City
  - Runs Left
  - Balls Left
  - Wickets Remaining
  - Current Run Rate (CRR)
  - Required Run Rate (RRR)
  - Total Target Runs

## Future Enhancements
- **Real-Time Data Fetching**: Integrate live match data via an API.
- **Match Progression Visualization**: Display graphs for run rate, win probability, and wickets over time.
- **More Advanced ML Models**: Experiment with Random Forest, XGBoost, or Deep Learning for better accuracy.

## Deployment Plan
- Deploy using **Render / Hugging Face Spaces / Streamlit Cloud**.
- Store the trained model (`pipe.pkl`) in the repository for easy access.
- Ensure proper UI enhancements for a smooth experience.

## Contributing
Feel free to fork this project and contribute by adding new features! 🚀

## Author
- **Rohan Soni**
- GitHub: [Rohansoni45](https://github.com/Rohansoni45)
- LinkedIn: [Rohan soni](https://www.linkedin.com/in/rohansoni9475/)

## License
This project is open-source and available under the MIT License.

