# ACN - SAP HR/Payroll ABAP Repository

**Accenture Contingent Workforce Management - HR Payroll Systems**

This repository contains SAP ABAP reports, function modules, and master data configurations for HR and payroll processing. All files are organized for easy access and reference.

---

## 📋 Table of Contents

- [Reports & Documents](#reports--documents)
- [Function Modules](#function-modules)
- [Configuration Files](#configuration-files)
- [How to Use](#how-to-use)
- [Repository Structure](#repository-structure)

---

## 📊 Reports & Documents

### Master Data Reports

| Report ID | Document | Purpose | Format |
|-----------|----------|---------|--------|
| **ZRPPA0074** | [Consolidated Master Data Report](./Consolidated%20master%20data%20report%20ZRPPA0074.pdf) | Consolidates employee master data, organizational structure, and payroll configuration | PDF |
| **ZRPPA0087** | [Long Service Award Report](./ZRPPA0087%20long%20service%20award.pdf) | Identifies employees eligible for long service awards and benefits | PDF |
| **ZRPPA0088** | [Honeywell Interface](./ZRPPA0088%20Honeywell%20Interface.pdf) | Integration specifications for Honeywell systems | PDF |
| **ZRPPA0096** | [Contract Expiry Report](./ZRPPA0096%20Contract%20expiry.pdf) | Lists contracts approaching expiration dates | PDF |
| **ZRPPA0098** | [Confidentiality Agreement](./ZRPPA0098%20Confid%20agreement.pdf) | Standard confidentiality and NDA documentation | PDF |

### Payroll & Compensation

| Report ID | Document | Purpose | Format |
|-----------|----------|---------|--------|
| **ZRPPY0267** | [Annual Earnings Report](./ZRPPY0267%20ANNUAL%20EARNINGS%20REPORT%20PDF%20EMAIL.pdf) | Comprehensive annual earnings and compensation details | PDF |
| **ZRPPY0363** | [Employee CTS Slip](./ZRPPY0363%20Employee%20CTS%20Slip.pdf) | Cash Throgh Settlement slip for employee compensation | PDF |

### HR Management

| Document | Purpose | Format |
|----------|---------|--------|
| [HR Managers Reference](./ZREAD_MANAGERS.pdf) | HR manager roles, responsibilities, and access controls | PDF |

---

## 🔧 Function Modules

### PDF & File Handling

| Module Name | Document | Purpose | Format |
|-------------|----------|---------|--------|
| **Z_FILE_PDF_ENCRYPT** | [PDF Encryption Module](./Z_FILE_PDF_ENCRYPT%20FM.pdf) | Encrypts PDF files for secure transmission | PDF |

### Manager & HR Data Retrieval

| Module Name | Document | Purpose | Format |
|-------------|----------|---------|--------|
| **ZSWX_GET_DIRECT_MANAGER** | [Direct Manager Retrieval FM](./ZSWX_GET_DIRECT_MANAGER%20FM.pdf) | Retrieves direct manager information from employee records | PDF |
| **ZSWX_GET_DIRECT_MANAGER** (Code) | [Direct Manager Code Documentation](./ZSWX_GET_DIRECT_MANAGER%20FM_code.pdf) | ABAP source code and technical implementation details | PDF |
| **Z_GET_HR_MANAGER** | [HR Manager Retrieval FM](./Z_GET_HR_MANAGER.pdf) | Fetches HR manager assigned to department or employee | PDF |
| **Z_GET_HR_MANAGER** (Code) | [HR Manager Code Documentation](./Z_GET_HR_MANAGER%20FM_code.pdf) | Complete ABAP implementation and usage examples | PDF |

---

## ⚙️ Configuration Files

### Master Data Configuration

| File Name | Purpose | Format | Content Type |
|-----------|---------|--------|---------------|
| [zsfppa_masterdata consolidated.xml](./zsfppa_masterdata%20consolidated.xml) | Central master data configuration combining employee, organizational, and payroll settings | XML | Configuration |

### Form Templates & Adobe Integration

| File Name | Purpose | Format | Content Type |
|-----------|---------|--------|---------------|
| [SFPF_ZPY_AFP_CTS_FORM adobe ZRPPY0363 form.XML](./SFPF_ZPY_AFP_CTS_FORM%20%20adobe%20ZRPPY0363%20form%20.XML) | Adobe Form Designer template for CTS (Cash Through Settlement) employee slips | XML | Form Template |

---

## 📖 How to Use

### For ABAP Developers

1. **View Function Module Documentation:**
   - Click on any `FM.pdf` link to see function specifications
   - Click on any `FM_code.pdf` link to see ABAP source code

2. **Import Function Modules:**
   - Use Transaction `SE38` (ABAP Editor) or `SE80` (ABAP Workbench)
   - Reference the code documentation for implementation details

3. **Configure Master Data:**
   - Open `zsfppa_masterdata consolidated.xml`
   - Update settings according to your system requirements
   - Import via Transaction `SE38` or custom transport

### For HR Business Users

1. **Run Reports:**
   - Open SAP Transaction `SE38`
   - Enter report name (e.g., `ZRPPA0074`)
   - Select required period and parameters
   - Execute and download results

2. **Access Employee Slips:**
   - Navigate to relevant payroll transaction
   - Use `ZRPPY0363` for employee CTS slip generation
   - Download PDF for distribution

3. **Review Master Data:**
   - Use `ZRPPA0074` for consolidated view
   - Cross-reference with configuration file `zsfppa_masterdata consolidated.xml`

### For System Administrators

1. **Implement Function Modules:**
   - Review documentation in `Z_GET_HR_MANAGER FM.pdf`
   - Deploy code using Transport Management System (TMS)
   - Test in DEV/QA before production

2. **Configure Forms:**
   - Edit Adobe forms using `ZRPPY0363` form template
   - Test with sample data
   - Deploy to production environment

3. **Maintain Integrations:**
   - Reference `ZRPPA0088 Honeywell Interface.pdf` for third-party system connections
   - Use `Z_FILE_PDF_ENCRYPT` for secure document handling

---

## 📁 Repository Structure

```
ACN/
├── README.md                                    # This file
├── 
├── 📊 MASTER DATA REPORTS
├── ├── Consolidated master data report ZRPPA0074.pdf
├── ├── ZRPPA0087 long service award.pdf
├── ├── ZRPPA0088 Honeywell Interface.pdf
├── ├── ZRPPA0096 Contract expiry.pdf
├── └── ZRPPA0098 Confid agreement.pdf
├──
├── 💰 PAYROLL & COMPENSATION
├── ├── ZRPPY0267 ANNUAL EARNINGS REPORT PDF EMAIL.pdf
├── ├── ZRPPY0363 Employee CTS Slip.pdf
├── └── ZREAD_MANAGERS.pdf
├──
├── 🔧 FUNCTION MODULES (FM)
├── ├── Z_FILE_PDF_ENCRYPT FM.pdf
├── ├── ZSWX_GET_DIRECT_MANAGER FM.pdf
├── ├── ZSWX_GET_DIRECT_MANAGER FM_code.pdf
├── ├── Z_GET_HR_MANAGER.pdf
├── └── Z_GET_HR_MANAGER FM_code.pdf
├──
└── ⚙️ CONFIGURATION
    ├── zsfppa_masterdata consolidated.xml
    └── SFPF_ZPY_AFP_CTS_FORM adobe ZRPPY0363 form.XML
```

---

## 🎯 Quick Links by Role

### **ABAP Developer**
- [Z_GET_HR_MANAGER Function Module](./Z_GET_HR_MANAGER.pdf)
- [Z_GET_HR_MANAGER Source Code](./Z_GET_HR_MANAGER%20FM_code.pdf)
- [Direct Manager Retrieval FM](./ZSWX_GET_DIRECT_MANAGER%20FM.pdf)
- [PDF Encryption Module](./Z_FILE_PDF_ENCRYPT%20FM.pdf)
- [Master Data Configuration](./zsfppa_masterdata%20consolidated.xml)

### **HR Business Analyst**
- [Consolidated Master Data Report](./Consolidated%20master%20data%20report%20ZRPPA0074.pdf)
- [Long Service Award Report](./ZRPPA0087%20long%20service%20award.pdf)
- [Employee CTS Slip](./ZRPPY0363%20Employee%20CTS%20Slip.pdf)
- [Annual Earnings Report](./ZRPPY0267%20ANNUAL%20EARNINGS%20REPORT%20PDF%20EMAIL.pdf)
- [Contract Expiry Report](./ZRPPA0096%20Contract%20expiry.pdf)

### **System Administrator**
- [HR Manager Reference](./ZREAD_MANAGERS.pdf)
- [Honeywell Interface Documentation](./ZRPPA0088%20Honeywell%20Interface.pdf)
- [Master Data Configuration](./zsfppa_masterdata%20consolidated.xml)
- [CTS Form Template](./SFPF_ZPY_AFP_CTS_FORM%20%20adobe%20ZRPPY0363%20form%20.XML)

---

## 📝 File Naming Convention

All files follow SAP naming standards:

- **Z* Prefix:** Custom developments (not SAP standard)
- **ZRPPA* :** Reports for HR Master Data
- **ZRPPY* :** Reports for Payroll
- **Z*_FM :** Function Module documentation
- **Z*_FM_code :** Function Module source code

---

## ⚠️ Important Notes

- **Confidential:** This repository contains sensitive HR and payroll information. Access should be restricted to authorized personnel only.
- **Testing:** Always test changes in DEV/QA environment before deploying to production.
- **Backups:** Maintain regular backups of all configuration files and master data.
- **Compliance:** Ensure all payroll processing complies with local labor laws and regulations.

---

## 🔗 Related Resources

- **SAP Transactions Used:**
  - SE38: ABAP Report Editor
  - SE80: ABAP Object Navigator
  - PA30: HR Master Record
  - PY01: Payroll Configuration

- **Key Modules:**
  - HR-Master Data Management
  - Payroll Processing
  - Forms & Document Management

---

## 📞 Support

For questions or issues related to these reports and function modules, please contact:

- **HR Systems Team:** [Email/Contact]
- **ABAP Development Team:** [Email/Contact]
- **Repository Maintainer:** KundanP-ai

---

## 📄 Document History

| Date | Version | Description |
|------|---------|-------------|
| 2026-05-23 | 1.0 | Initial README creation with all file links and documentation |

---

**Last Updated:** 2026-05-23  
**Repository Owner:** KundanP-ai  
**Organization:** Accenture (ACN)
