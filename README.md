# 🌐 NetScope — Local Network Service Reporter

**NetScope** is a Flask-based local network scanning and service reporting tool. It uses **Nmap** to discover hosts, detect open ports and identify available network services, then presents the results through a simple web interface.

## ✨ Features

- 🔍 Local network / host scanning with Nmap
- 📡 Open port and service detection
- 📊 Web-based scan results
- 📄 PDF report generation
- 🧾 XML report generation
- 📥 Report download support
- 🗄️ Local database support for scan/report data
- 📱 Responsive dark-themed interface

## 🛠️ Technologies Used

- **Python**
- **Flask**
- **Nmap**
- **HTML5 / CSS3**
- **SQLite**
- **ReportLab / XML reporting**

## 📁 Project Structure

```text
NetScope/
│
├── app.py                  # Main Flask application
├── database.py             # Database operations
├── email_report.py         # Email/report functionality
├── pdf_report.py           # PDF report generation
├── xml_report.py           # XML report generation
├── recommendations.py      # Service/security recommendations
├── scanner_test.py         # Scanner testing
├── requirements.txt        # Required Python packages
├── netscope.db             # Local database
├── README.md               # Project documentation
│
├── scanner/
│   └── ...                 # Nmap scanning modules
│
├── templates/
│   └── ...                 # HTML pages
│
├── static/
│   └── style.css           # Website styling
│
├── reports/
│   └── ...                 # Generated reports
│
└── docs/
    └── ...                 # Project screenshots / documentation
```

## 🔎 Nmap

NetScope uses **Nmap (Network Mapper)** as its scanning engine.

Nmap is responsible for discovering hosts, checking ports and identifying services running on the target system.

NetScope sends the required scan request to Nmap, processes the returned information and displays the results in the web interface.

> ⚠️ Use NetScope and Nmap only on systems and networks you own or have permission to test.

## 🚀 Installation

### 1. Clone the repository

```bash
git clone https://github.com/Paramasivam23/netscope-reporter.git
cd netscope-reporter
```

### 2. Install Python dependencies

```bash
pip install -r requirements.txt
```

### 3. Make sure Nmap is installed

Install Nmap on your system and make sure the `nmap` command is available from the terminal.

Check with:

```bash
nmap --version
```

### 4. Run NetScope

```bash
python app.py
```

Open the local address shown in the terminal, usually:

```text
http://127.0.0.1:5000
```

## 📊 Reports

NetScope can generate scan reports in different formats, including:

- PDF
- XML

Generated reports are stored in the project's `reports/` directory.

## 🖼️ Screenshots

Project screenshots are maintained inside the `docs/` directory.

The screenshots demonstrate the main interface, scanning workflow and generated results/reports.

## 📌 Project Status

**Status: Completed / Working**

The implemented application supports network scanning, service detection, web-based result display and report generation.

## 🔗 GitHub Repository

**NetScope — Local Network Service Reporter**

https://github.com/Paramasivam23/netscope-reporter

## 👨‍💻 Author

**Paramasivam m**

---

> **Note:** NetScope is intended for authorized network testing and educational purposes only.
