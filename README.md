## **Task 1: All Standards Books**

### **Dashboard Options:**

The main dashboard displays the following options:

1. **Prathmik Vibhag** (Primary Section)
2. **Uchhatar Prathmik Vibhag** (Upper Primary Section)
3. **Madhyamik Vibhag** (Secondary Section)
4. **Uchhatar Madhyamik Vibhag** (Higher Secondary Section)

---

### **Functionality Flow:**

1. **Dashboard Options:**

   - When the user clicks on any of the above sections, it will show all the standards that belong to the clicked section.
   - This is done by fetching standards where the `dashboard_option_id` matches the clicked section.
     - **Example:** Clicking **Prathmik Vibhag** will show standards from **1 to 5**.

2. **Standards:**

   - When a user selects a standard, the app displays all books associated with that **standard.id**.

3. **Books:**

   - Clicking on a book will show all chapters related to that book.
   - Each chapter provides three options:
     - **View:** Opens a PDF of the book at the specified page number.
     - **YouTube:** Opens a new screen with all YouTube videos for the selected chapter.
     - **Swadhyay:** Opens a Swadhyay PDF of the chapter.

---

### **Backend APIs:**

All APIs are hosted at: **`rrr.jatssdev.com/api/`**

| **API Endpoint** | **Description**                           | **Usage**                                                |
| ---------------- | ----------------------------------------- | -------------------------------------------------------- |
| `/standard/all`  | Fetches all standards.                    | Used to display standards after selecting a section.     |
| `/book/all`      | Fetches all books.                        | Used after selecting a standard to show relevant books.  |
| `/chapter/all`   | Fetches all chapters of a book.           | Used after selecting a book to display chapters.         |
| `/youtube/all`   | Fetches all YouTube videos for a chapter. | Displays YouTube videos under the YouTube option.        |
| `/swadhyay/all`  | Fetches all Swadhyay PDFs for a chapter.  | Opens Swadhyay PDFs when the Swadhyay option is clicked. |

---

### **File URLs:**

- All API files are stored on the server under the directory: **rrr.jatssdev.com/api**

#### **API File Paths:**

- Standards API: `/standard/all`
- Books API: `/book/all`
- Chapters API: `/chapter/all`
- YouTube API: `/youtube/all`
- Swadhyay API: `/swadhyay/all`

#### **Books and Chapters File Paths:**

- **Books & Chapters (Images/PDFs):**\
  `rrr.jatssdev.com/uploads/{image_or_pdf_name}`





---

## **Task 2: Bhagwad Geeta Section**

### **Dashboard Option:**

The main dashboard also includes:

5. **Bhagwad Geeta**

---

### **Functionality Flow:**

1. **Bhagwad Geeta Option:**

   - When the user clicks on the **Bhagwad Geeta** option, it will fetch and display all content using the following API:
     - **API:** `https://rrr.jatssdev.com/api/bhagwad-geeta/all`
   - Each fetched item includes an icon and a PDF URL.

2. **View Option:**

   - The **View** option will open a PDF viewer to display the corresponding Bhagwad Geeta PDF.

---

### **Backend API:**

All APIs are hosted at: **`rrr.jatssdev.com/api/`**

| **API Endpoint**     | **Description**                | **Usage**                                            |
| -------------------- | ------------------------------ | ---------------------------------------------------- |
| `/bhagwad-geeta/all` | Fetches Bhagwad Geeta content. | Displays Bhagwad Geeta items with a PDF view option. |

---

### **File URLs:**

- All API files are stored on the server under the directory: \`\`

#### **Bhagwad Geeta File Paths:**

- **PDFs & Icons:**\
  `rrr.jatssdev.com/geeta/{pdf_or_icon_name}`
