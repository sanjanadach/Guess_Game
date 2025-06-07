import streamlit as st
import random

st.title("🎯 Number Guessing Game")
st.write("Guess a number between 1 and 100!")

# Initialize session state
if "number" not in st.session_state:
    st.session_state.number = random.randint(1, 100)
if "guessed" not in st.session_state:
    st.session_state.guessed = False

# Input for user guess
guess = st.number_input("Enter your guess:", min_value=1, max_value=100, step=1)

if st.button("Guess"):
    if guess == st.session_state.number:
        st.success(f"🎉 Correct! The number was {st.session_state.number}")
        st.session_state.guessed = True
    elif guess < st.session_state.number:
        st.warning("Too low! Try again.")
    else:
        st.warning("Too high! Try again.")

if st.session_state.guessed:
    if st.button("Play Again"):
        st.session_state.number = random.randint(1, 100)
        st.session_state.guessed = False
        st.experimental_rerun()
