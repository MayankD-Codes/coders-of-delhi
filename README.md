# Coders of Delhi

## 📌 Project Overview
**Coders of Delhi** is an **end-to-end data science project** simulating a mini social network for coders.  
The project demonstrates data cleaning, friendship recommendation, and content/page recommendation systems — all implemented in **pure Python** without external machine learning libraries.

---

## 🎯 Features Implemented

### 1. **Data Cleaning**
- Loaded messy JSON data from the social network simulation.
- Removed duplicates, fixed formatting issues, and standardized structure.
- Exported cleaned data to `cleaned_codebook_data.json`.

### 2. **People You May Know**
- Suggested potential friends based on **mutual friends count**.
- Higher number of mutual friends → higher recommendation priority.
- Implemented ranking logic for recommendations.

### 3. **Pages You Might Like**
- Used a **collaborative filtering approach** to recommend pages.
- If two users like the same pages, they may also like other pages liked by each other.
- Scored recommendations by number of common liked pages.

---

## 🛠️ Tech Stack
- **Language:** Python 3
- **Data Format:** JSON
- **Libraries Used:** Only Python Standard Library (`json`, `set`, sorting logic)

---

## 📂 Project Structure
coders-of-delhi/
│
├── 01_clean_data.py # Cleans and structures raw JSON data
├── 02_people_you_may_know.py # Suggests friends using mutual connections
├── 03_pages_you_might_like.py # Recommends pages using collaborative filtering
├── codebook_data.json # Original dataset
├── cleaned_codebook_data.json # Cleaned dataset
└── README.md # Project documentation

yaml
Copy
Edit

---

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/MayankD-Codes/coders-of-delhi.git
   cd coders-of-delhi
Ensure Python 3 is installed:

bash
Copy
Edit
python --version
Run scripts in order:

bash
Copy
Edit
python 01_clean_data.py
python 02_people_you_may_know.py
python 03_pages_you_might_like.py
📊 Example Output
People You May Know

less
Copy
Edit
People You May Know for User 1: [4]
Pages You Might Like

sql
Copy
Edit
Pages You Might Like for User 1: [103]
📜 License
This project is open-source and free to use for educational purposes.
