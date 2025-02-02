# StrumAlign2 Documentation

## Overview
StrumAlign2 is a project designed to detect and align guitar strumming patterns using a machine learning model. It consists of a frontend built with React (Vite) and a backend that includes a trained PyTorch model for chord detection.

---

## Project Structure

### **Frontend (Client) - React & Vite**
- **Main Files:**
  - `index.html` - Main HTML template.
  - `src/App.jsx` - Root React component.
  - `src/components/Navbar.jsx` - Navigation bar component.
  - `src/pages/`
    - `Chord.jsx` - Likely responsible for chord-related functionalities.
    - `Home.jsx` - Main landing page.
    - `Record.jsx` - Recording page for capturing audio input.
  
- **Styling:**
  - `App.css`, `index.css` - Styles for the application.
  - TailwindCSS configured via `tailwind.config.js`.
  
- **Configuration:**
  - `package.json` - Lists dependencies and scripts.
  - `vite.config.js` - Configuration for Vite.
  - `.gitignore` - Git version control settings.

---

### **Backend (Server) - Python**

#### **Machine Learning Model**
- `guitar_chord_model.pth` - Pre-trained PyTorch model for detecting guitar chords.
- `train_chord.ipynb` - Jupyter Notebook used for training the model.

#### **Key Scripts**
- `chord_detection.py` - Responsible for detecting chords, likely using the trained model.
- `handtracker.py` - Potentially tracks finger positions for detecting correct chord playing.

---

## **Installation & Setup**

### **Frontend Setup**
```bash
cd client
npm install
npm run dev
```

### **Backend Setup**
```bash
cd server
pip install -r requirements.txt  # Ensure dependencies are installed
python chord_detection.py  # Run the backend
```

---

## **Usage Guide**
1. Run the backend using `python chord_detection.py`.
2. Start the frontend using `npm run dev`.
3. Access the application via the browser to detect chords using the trained ML model.

---

## **Future Enhancements**
- Improve chord detection accuracy.
- Integrate real-time feedback for users.
- Add support for multiple instruments.

---

## **Contributors**
- **Developers:** Aditya Kidiyoor, Sanika Chimurkar, Malavika Saritha

For additional support, refer to the project repository or contact the maintainers.
