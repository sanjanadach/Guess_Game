## 🎯 Number Guessing Game (Streamlit)
This is a simple and interactive web app built using Streamlit where users try to guess a randomly generated number between 1 and 100. Great for learning how to use st.session_state to maintain state in Streamlit apps!

## 🚀 Features
Random number is generated on each game start.

User receives feedback whether their guess is too low, too high, or correct.

Upon a correct guess, a "Play Again" button appears to restart the game.

Uses st.session_state to preserve game state between interactions.


## 🧩 How It Works
A random number between 1 and 100 is generated and stored in the session state.

The user inputs a number and clicks "Guess".

The app gives a hint:

🎯 Correct

🔽 Too low

🔼 Too high

After a correct guess, users can restart the game by clicking "Play Again".

## 🛠️ Installation & Running the App

🔧 Prerequisites
Python 3.7+

streamlit library

## 📦 Installation
bash

Copy

Edit

pip install streamlit

▶️ Run the App
bash

Copy

Edit

streamlit run app.py

## 📁 File Structure
text
Copy
Edit
📦number-guessing-game

 ┣ 📄 app.py            # Streamlit main application file
 
 ┗ 📄 README.md         # This file
 
🙌 Acknowledgements

Thanks to the Streamlit team for making web app development in Python super easy and fun!



