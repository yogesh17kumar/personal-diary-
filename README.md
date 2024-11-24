import streamlit as st
import os
from datetime import datetime

DIARY_FILE = "diary.txt"

# Title
st.title("📖 Personal Diary App")

# Sidebar Navigation
st.sidebar.title("Navigation")
page = st.sidebar.radio("Go to", ["Write Entry", "View Entries", "Search Entries", "Delete All Entries"])

# Write Entry Page
if page == "Write Entry":
    st.header("✍️ Write a New Diary Entry")
    current_date = datetime.now().strftime("%Y-%m-%d")
    date = st.text_input("Date (YYYY-MM-DD):", value=current_date)
    entry = st.text_area("Write your diary entry here:")

    if st.button("Save Entry"):
        if date.strip() and entry.strip():
            with open(DIARY_FILE, "a") as file:
                file.write(f"Date: {date}\n{entry}\n{'-'*40}\n")
            st.success("✅ Entry saved successfully!")
        else:
            st.error("❌ Date and Entry cannot be empty!")

# View Entries Page
elif page == "View Entries":
    st.header("📚 View All Diary Entries")
    if os.path.exists(DIARY_FILE):
        with open(DIARY_FILE, "r") as file:
            entries = file.read()
        st.text_area("All Entries", entries, height=300)
    else:
        st.info("ℹ️ No entries found. Start writing your diary!")

# Search Entries Page
elif page == "Search Entries":
    st.header("🔍 Search Diary Entries")
    query = st.text_input("Search by date or keyword:")
    if st.button("Search"):
        if os.path.exists(DIARY_FILE):
            with open(DIARY_FILE, "r") as file:
                entries = file.read().split("\n" + "-"*40 + "\n")
            results = [entry for entry in entries if query in entry]
            if results:
                st.success(f"✅ Found {len(results)} result(s):")
                for result in results:
                    st.text_area("Result", result, height=150)
            else:
                st.warning("⚠️ No entries found matching your query.")
        else:
            st.info("ℹ️ No entries found. Start writing your diary!")

# Delete All Entries Page
elif page == "Delete All Entries":
    st.header("🗑️ Delete All Entries")
    if st.button("Delete All Entries"):
        if os.path.exists(DIARY_FILE):
            os.remove(DIARY_FILE)
            st.success("✅ All entries deleted successfully!")
        else:
            st.info("ℹ️ No entries found to delete.")

# Footer
st.sidebar.write("Developed with ❤️ using Streamlit")
