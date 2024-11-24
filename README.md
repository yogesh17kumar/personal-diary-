<<<<<<< HEAD
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Documentation for the Personal Diary Application built with Python and Tkinter.">
    <title>Personal Diary Application - Documentation</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0 auto;
            max-width: 800px;
            padding: 20px;
            background-color: #f4f4f9;
            color: #333;
        }
        h1, h2, h3 {
            color: #444;
        }
        code {
            background-color: #e8e8e8;
            padding: 2px 5px;
            font-family: Consolas, monospace;
            border-radius: 3px;
            font-size: 90%;
        }
        pre {
            background-color: #f1f1f1;
            padding: 15px;
            border-radius: 5px;
            overflow-x: auto;
            border: 1px solid #ddd;
        }
        ul, ol {
            margin: 10px 0 20px 20px;
        }
        a {
            color: #007BFF;
            text-decoration: none;
        }
        a:hover {
            text-decoration: underline;
        }
        .button {
            display: inline-block;
            padding: 8px 12px;
            margin: 10px 0;
            font-size: 14px;
            color: #fff;
            background-color: #007BFF;
            text-align: center;
            border: none;
            border-radius: 4px;
            text-decoration: none;
            cursor: pointer;
        }
        .button:hover {
            background-color: #0056b3;
        }
        .highlight {
            color: #e63946;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1>Personal Diary Application</h1>
    <p>This application is a GUI-based personal diary tool developed in Python using <code>Tkinter</code>. It enables users to save, view, search, and delete diary entries while maintaining simplicity and ease of use.</p>

    <h2>Features</h2>
    <ul>
        <li><strong>Save Entries:</strong> Write and save diary entries with timestamps.</li>
        <li><strong>View Entries:</strong> Display all saved diary entries in a scrollable popup window.</li>
        <li><strong>Search Entries:</strong> Search for diary entries by date or keywords.</li>
        <li><strong>Delete Entries:</strong> Delete all saved entries with a confirmation prompt.</li>
        <li><strong>Exit:</strong> Close the application gracefully.</li>
    </ul>

    <h2>Requirements</h2>
    <ul>
        <li>Python 3.x installed on your system.</li>
        <li>No additional libraries required (uses Python's built-in <code>Tkinter</code> module).</li>
    </ul>

    <h2>How to Run</h2>
    <ol>
        <li>Download or copy the Python script (<code>personal_diary.py</code>).</li>
        <li>Ensure Python 3.x is installed on your computer.</li>
        <li>Run the script using the command:
            <pre>python personal_diary.py</pre>
        </li>
        <li>The application window will open, allowing you to interact with the diary.</li>
    </ol>

    <h2>Usage Instructions</h2>
    <h3>1. Save a Diary Entry</h3>
    <ol>
        <li>Enter the date in <code>YYYY-MM-DD</code> format (default is the current date).</li>
        <li>Write your diary content in the provided text area.</li>
        <li>Click the <strong>Save Entry</strong> button to save your entry.</li>
    </ol>

    <h3>2. View Saved Entries</h3>
    <ul>
        <li>Click the <strong>View Entries</strong> button to display all previously saved entries.</li>
        <li>A scrollable popup window will show the content.</li>
    </ul>

    <h3>3. Search for an Entry</h3>
    <ul>
        <li>Enter a date (e.g., <code>2024-11-23</code>) or a keyword in the search field.</li>
        <li>Click the <strong>Search Entry</strong> button to find matching entries.</li>
        <li>Results will be displayed in a popup window. If no match is found, an alert will inform you.</li>
    </ul>

    <h3>4. Delete All Entries</h3>
    <ul>
        <li>Click the <strong>Delete Entries</strong> button to remove all saved entries.</li>
        <li>You will be prompted to confirm this action. Choose <span class="highlight">Yes</span> to proceed.</li>
    </ul>

    <h3>5. Exit the Application</h3>
    <ul>
        <li>Click the <strong>Exit</strong> button to close the application.</li>
    </ul>

    <h2>File Structure</h2>
    <ul>
        <li><code>personal_diary.py</code>: The main Python script for the application.</li>
        <li><code>diary.txt</code>: A text file where all diary entries are stored (created automatically).</li>
    </ul>

    <h2>Example</h2>
    <h3>Save an Entry</h3>
    <pre>
Date: 2024-11-23
Entry: "Today I completed a personal project and felt very productive!"
    </pre>
    <h3>Search Results</h3>
    <pre>
Date: 2024-11-23
Entry: "Today I completed a personal project and felt very productive!"
    </pre>

    <h2>Error Handling</h2>
    <ul>
        <li>Prompts users to fill in missing fields (date or diary content).</li>
        <li>Handles missing <code>diary.txt</code> file by creating a new one.</li>
        <li>Ensures proper formatting for date input (<code>YYYY-MM-DD</code>).</li>
    </ul>

    <h2>Future Enhancements</h2>
    <ul>
        <li>Enable password protection for accessing the diary.</li>
        <li>Add text formatting options (e.g., bold, italic, underline).</li>
        <li>Provide an export feature to save entries as PDFs.</li>
        <li>Include categories/tags for diary entries for easier searching.</li>
    </ul>

    <h2>Contact</h2>
    <p>For suggestions, feedback, or reporting bugs, please contact:</p>
    <ul>
        <li><strong>Email:</strong> developer@example.com</li>
        <li><strong>GitHub:</strong> <a href="https://github.com" target="_blank">Visit Profile</a></li>
    </ul>

    <p style="text-align: center;">✨ <strong>Happy Journaling!</strong> ✨</p>
</body>
</html>
=======
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
