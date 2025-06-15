# 📦 File Compression Web App

A full-stack web application that allows users to upload files and apply compression algorithms like **Huffman Coding**, **Run-Length Encoding (RLE)**, and **LZ77**. The app visualizes compression statistics, shows algorithm details, and enables downloading compressed or decompressed files.

---

## 🌐 Live Demo

https://youtu.be/ZZXEGXDISD8

---

## 📸 Screenshots

### 🔹 Home & File Upload Interface
Upload Section 

(https://github.com/user-attachments/assets/5ebbc2c7-84c9-4669-a1ea-4c2e3c16baa6)

Algorithm Selection

(https://github.com/user-attachments/assets/ce45c483-1f0f-49e0-a520-b4116c8d4ddd)

### 🔹 Algorithm Description Modal

(https://github.com/user-attachments/assets/aa853ff6-6123-4979-b1c2-99948229c576)

### 🔹 Compression Statistics

(https://github.com/user-attachments/assets/3dc164da-cbb3-449e-a399-616022f6d0f0)


### 🔹 Final Result with Download

Download Compressed File

---

## 🧠 Features

- 📁 **File Upload** – Upload text, image, or binary files
- 🧠 **Choose Algorithm** – Huffman, RLE, or LZ77
- 📉 **Real-Time Statistics** – View original vs compressed size, time, and ratio
- 🔍 **Algorithm Explanation** – Understand how each algorithm works
- 📥 **Download Option** – Save the compressed/decompressed file
- 🧩 **Modular Codebase** – Clean and reusable component structure
- ⚠️ **Error Handling** – Informative feedback for unsupported actions
- 📱 **Responsive UI** – Built with Tailwind CSS for mobile-friendly experience

---

## 🏗️ Project Structure

src/
├── components/ # Reusable UI components
│ ├── AlgorithmDescription.jsx
│ ├── AlgorithmSelector.jsx
│ ├── FileDownloader.jsx
│ ├── FileUploader.jsx
│ └── StatsDisplay.jsx
├── hooks/ # Custom React hooks
│ ├── use-mobile.jsx
│ └── use-toast.js
├── pages/ # Page-level components
│ ├── Index.jsx
│ └── NotFound.jsx
├── utils/ # Compression algorithms
│ ├── huffman.js
│ ├── lz77.js
│ └── rle.js
├── App.jsx # Main application
├── main.jsx # Entry point
├── App.css / index.css # Styling

yaml
Copy
Edit

---

## 🛠️ Tech Stack

### Frontend:
- **React.js** with **Vite**
- **Tailwind CSS** for responsive design
- **Recharts** for visual graphs
- **FileReader API** for in-browser file parsing

### Backend (optional):
- Compression is done fully in-browser using custom JS modules.
- Can be extended with Node.js or Python for larger or secured file handling.

---

## ⚙️ Installation & Setup

```bash
# Clone the repository
git clone https://github.com/your-username/compression-app.git
cd compression-app

# Install dependencies
npm install

# Start development server
npm run dev
📚 Supported Algorithms
🔵 Huffman Coding
How it works: Builds a binary tree using character frequencies to assign variable-length codes.

Best for: Text, structured files

🔵 Run-Length Encoding (RLE)
How it works: Encodes repeated characters as a single character + count.

Best for: Simple graphics, repetitive content

🔵 LZ77
How it works: Uses a sliding window to refer back to repeated sequences.

Best for: Mixed content types

📊 Example Output
Original Size: 3.37 KB

Compressed Size: 1.91 KB

Compression Ratio: 1.77:1 (43.4% space saved)

Processing Time: 47ms

✅ Future Improvements
Drag-and-drop support

More algorithms (LZW, BWT)

Backend mode for large files

Dark mode toggle

History of previous compressions

📄 License
MIT License © 2025 Piyush Bhaskar

🙌 Acknowledgements
React & Vite

Tailwind CSS

Recharts

Lucide Icons
