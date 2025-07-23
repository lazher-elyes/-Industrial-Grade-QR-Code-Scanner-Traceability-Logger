# Industrial-Grade QR Code Scanner & Traceability Logger

**Solving Industrial Product Traceability & Invalid QR Code Issues in Computer Vision Systems**

---

## Overview

In industrial production and quality control, computer vision systems sometimes fail to recognize certain QR codes due to printing defects, lighting conditions, or scanning angle. However, manual handheld scanners can still read these codes reliably.

This project provides a robust **manual QR code scanning and logging solution** designed for industrial environments where:

- QR codes may be **invalid or problematic for automated vision systems**,  
- But **can still be reliably scanned manually** by operators.

It enables operators to quickly scan product codes, automatically generate verified QR code images, and keep a **detailed Excel log with embedded QR codes** for traceability and audit purposes.

---

## Key Benefits

- **Reliable manual scanning fallback** for problematic or invalid QR codes that fail automated vision systems.  
- **Automatic generation and archival of QR code images** alongside scan records for verification.  
- **Persistent duplicate prevention** across multiple scanning sessions to maintain data integrity.  
- **Instant data backup to prevent loss during interruptions or shutdowns.**  
- **Clear Excel reports** with timestamps and embedded QR images, facilitating quality audits and supplier communications.  
- **Easy integration** in industrial workflows with minimal training required.

---

## Features

- Enforces product code format via prefix validation (customizable).  
- Detects and rejects duplicate scans both in current and past sessions.  
- Saves QR code images in a dedicated folder for offline reference.  
- Generates an Excel file with:  
  - Serial number (N°)  
  - Scan timestamp  
  - Scanned code  
  - Embedded QR code image (scaled and formatted for clarity)  
- Automatically adjusts Excel layout for professional readability.  
- Immediate saving after each scan to protect data integrity.

---

## Installation & Requirements

- Python 3.x  
- Required packages:  
  - [qrcode](https://pypi.org/project/qrcode/)  
  - [openpyxl](https://pypi.org/project/openpyxl/)

Install dependencies via:

```bash
pip install qrcode[pil] openpyxl
