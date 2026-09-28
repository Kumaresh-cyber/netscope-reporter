# NetScope — Local Network Service Reporter

**Created by Kumaresh**

NetScope is a lightweight Flask-based network service reporting application. It uses Nmap to scan an authorized local or private-network target and presents discovered hosts, ports, protocols, services, and versions in a simple web interface.

## Features

- Local network service scanning with Nmap
- Host and service information
- TCP and UDP service summary
- Scan duration and statistics
- Scan history
- HTML, PDF, and XML report generation
- Defensive security recommendations
- Clean web-based interface

## Nmap

NetScope uses **Nmap (Network Mapper)** for network discovery and service detection.

The application processes Nmap scan results and displays them in a readable format. Some scan features may require elevated privileges; when necessary, the application can use a TCP service-scan fallback.

> Only scan systems and networks that you own or have explicit permission to test.

## Project Structure

```text
NetScope/
├── app.py
├── database.py
├── requirements.txt
├── scanner/
│   ├── __init__.py
│   └── ...
├── reports/
├── templates/
│   ├── base.html
│   ├── index.html
│   ├── results.html
│   └── history.html
└── static/
    └── style.css
```

## Requirements

- Python 3
- Flask
- Nmap
- Python packages listed in `requirements.txt`

## Setup

```bash
pip install -r requirements.txt
```

Make sure Nmap is installed and available on your system.

## Run

```bash
python app.py
```

Open:

```text
http://127.0.0.1:5000
```

## Usage

1. Open the Scanner page.
2. Enter an authorized target address.
3. Start the scan.
4. Review detected hosts and services.
5. Open Scan History for previous scans.
6. Download the generated reports when required.

## Reports

NetScope supports:

- HTML reports
- PDF reports
- XML reports

---

**NetScope — Local Network Service Reporter**  
**Created by Kumaresh**
