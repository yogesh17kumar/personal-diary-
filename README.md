### **Personal Diary Application**

---

#### **Overview**

The **Personal Diary Application** is a Python-based GUI tool built using **Tkinter**. It allows users to maintain a digital diary for saving, viewing, searching, and managing daily entries. Each entry is timestamped with a date, making it an ideal solution for personal record-keeping.

---

#### **Features**

1. **Save Entry**:
   - Write a diary entry for the specified date and save it to a file.
2. **View Entries**:
   - View all saved diary entries in a scrollable popup window.
3. **Search Entry**:
   - Search for specific entries using a date or keyword.
4. **Delete Entries**:
   - Clear all saved diary entries after confirmation.
5. **Exit**:
   - Close the application gracefully.

---

#### **Requirements**

1. Python 3.x installed on your system.
2. No additional dependencies required (uses the standard Python library).

---

#### **Usage**

1. **Run the Application**:
   - Save the script to a file, e.g., `PersonalDiary.py`.
   - Run the application using:
     ```bash
     python PersonalDiary.py
     ```

2. **Saving an Entry**:
   - Enter the date in the format **YYYY-MM-DD** or use the pre-filled current date.
   - Write your diary entry in the text box.
   - Click the **Save Entry** button to save it to `diary.txt`.

3. **Viewing Entries**:
   - Click the **View Entries** button to see all saved entries in a popup window.

4. **Searching for an Entry**:
   - Enter a date (e.g., `2024-11-23`) or a keyword in the date field.
   - Click **Search Entry** to find and display matching entries.

5. **Deleting All Entries**:
   - Click the **Delete Entries** button to remove all saved diary entries.
   - Confirm the deletion when prompted.

6. **Exiting the Application**:
   - Click the **Exit** button to close the application.

---

#### **File Structure**

- **`personal_diary.py`**:
  - Main script containing the application logic.
- **`diary.txt`**:
  - File where all diary entries are saved (created automatically when an entry is saved).

---

#### **Code Description**

- **`save_entry()`**:
  - Saves the diary entry with a timestamp into `diary.txt`.
- **`view_entries()`**:
  - Reads and displays all entries from `diary.txt`.
- **`search_entry()`**:
  - Searches for a specific entry by date or keyword.
- **`delete_entries()`**:
  - Deletes all entries after user confirmation.
- **`show_popup()`**:
  - Displays content (entries or search results) in a scrollable popup window.

---

#### **Example Usage**

1. **Save an Entry**:
   - Date: `2024-11-23`
   - Entry: *"Had a wonderful day exploring the park."*
   - Output: Entry saved in `diary.txt`.

2. **Search an Entry**:
   - Query: `2024-11-23`
   - Result: Displays the entry for November 23, 2024.

3. **View Entries**:
   - Displays all saved diary entries in a popup window.

---

#### **Error Handling**

1. **Empty Inputs**:
   - Prompts the user to enter a date or write a diary entry if either is left blank.
2. **Invalid Date Format**:
   - Ensures the date format matches `YYYY-MM-DD`.
3. **File Not Found**:
   - Handles scenarios where `diary.txt` does not exist.

---

#### **Enhancements (Future Scope)**

1. **Password Protection**:
   - Add a login screen for securing diary entries.
2. **Rich Text Editing**:
   - Enable text formatting options (e.g., bold, italic, etc.).
3. **Export Entries**:
   - Allow exporting entries to PDF or other formats.
4. **Category Tags**:
   - Let users categorize entries for easier searching.

---

#### **Contact**

For suggestions or issues, feel free to contact the developer:
- **Email**: yogeshkumar17082003@gmail.com
Enjoy maintaining your personal diary! 😊
>>>>>>> ce3f62002d4882b628273df283157203ce663f8e
