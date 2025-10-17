# 🏅 HG Certificate Generator

A feature-rich PHP web application for **bulk and individual certificate generation, management, and verification** — perfect for events, courses, training institutions, and organizations.

![HG Certificate Generator Banner](https://your-repo-image-url/banner.png)

---

## 🚀 Features

- **Bulk Upload & Generation**: Upload a CSV to generate hundreds of certificates or badges in one batch, with any column order, and automatic field mapping.
- **Professional Certificate Templates**: Supports design-ready templates and dynamic placeholder replacement for personalized output.
- **Beautiful UI**: Modern, responsive, and crafted for seamless desktop/mobile administration.
- **Email Integration**: Send certificates directly to recipients from the interface (requires SMTP config).
- **One-Click Download**: Recipients can download their own certificate as PNG/PDF.
- **Advanced Verification**: Anyone can verify a certificate using a unique link or certificate number.
- **Social Sharing**: Recipients can share certificates to LinkedIn, WhatsApp, Facebook, X, and more (auto-filled for LinkedIn UI).
- **Admin Dashboard**: Search, revoke, re-send, and filter certificates by batch ("grouped" by upload).

---

## 📂 Project Structure

/
├── admin/ # Admin dashboard & management tools

├── public/ # Public-facing certificate view & verification

├── classes/ # Core PHP classes (certificate, bulk upload, database, etc.)

├── config/ # Application config files

├── assets/ # Styles, icons, sample CSVs, images

├── includes/ # Shared UI components (header/footer)

├── README.md # (you are here)

└── ...

---

## ⚙️ Quick Start

### Download the Release Package

You **cannot clone** this project directly because this is inside a parent monorepo.  
Instead:

1. **Download the release archive** from the repo sidebar (e.g. `v1.1.rar`, `v2.1.rar`) in [`/HG-Certificate-Generator`](https://github.com/Charitardha555/Hackers-Gurukul/tree/main/HG-Certificate-Generator)
2. **Extract all files** in your web server environment (`htdocs/`, `www/`, etc.)

**Example:**
- [v2.1.rar](https://github.com/Charitardha555/Hackers-Gurukul/raw/main/HG-Certificate-Generator/v2.1.rar)
- *(Older releases available as `v1.0.rar`, `v1.1.rar`, ...)*

---


### 2. **Set Up Local Development Environment**

- Use [XAMPP](https://www.apachefriends.org/) / [Laragon](https://laragon.org/) / [MAMP](https://www.mamp.info/) or similar LAMP stack on your machine.
- Create a new MySQL database (`hg_certificates`, etc.) and import the supplied SQL schema from `/docs` or initial migration.

### 3. **Update Configuration**

- Edit `/config/config.php` and set your database credentials.
- Set up **SMTP email settings** in `/classes/Emailer.php` for bulk/individual email sending.

### 4. **Update URLs**

- After local testing, change all occurrences of `"localhost"` to your **production domain** in config/code.

---

## 🗂️ Bulk Upload & Sample CSV

1. Use the **Bulk Upload** page in the admin panel to download the latest **sample CSV template**, featuring:

    | Recipient.Name | Email | Template.ID | Certification.Name | Certification.Field | Issued.On | Expiration.Date | Certificate.Status | Badge | Additional.Notes |
    |----------------|-------|-------------|-------------------|--------------------|-----------|-----------------|--------------------|-------|------------------|
    | Jane Doe       | jane@example.com | 1 | Certificate of Achievement | Cybersecurity | 2025-10-20 | 2026-10-20 | active | Gold | Completed all practicals |

2. **Edit and re-upload** your CSV — columns can be in any order; extra columns are supported.

---

## ✅ Core Admin Features

- **List, search, and filter certificates** (by status, batch, recipient, etc.)
- **Batch (Bulk) Management:** All bulk uploads are categorized as "batches"; certificates can be listed, filtered, and managed per batch.
- **Individual Actions:** View, revoke, resend, download, and verify certificates.

---

## 💡 Customization & Extensions

- **Templates**: Design new certificate templates and upload or edit the `/Template.php` logic.
- **Add new fields** by expanding the sample CSV and mapping logic in `bulk_upload.php`.
- **Enable/Disable Features** (e.g., disable download/print for privacy, hide revoked certs from public).

---

## 🔒 Security & Privacy

- Only logged-in admins can create, revoke, or manage certificates.
- Recipients can only access their certificate using a unique certificate link or number.
- Data is validated for each uploaded batch to prevent injection or malformed entries.

---

## ✉️ SMTP Email Setup

Edit `/classes/Emailer.php` with your SMTP server details for automatic mailing.

---

## 🌍 Demo & Live Usage

- Local: [http://localhost/public/](http://localhost/public/)
- **Replace localhost** with your own production hostname after deployment.

---

## 🛠️ Contributing

Pull requests, issues, and feedback are welcome! See [CONTRIBUTING.md](CONTRIBUTING.md) for details.

---

## 📃 License

Distributed under the MIT License. See [LICENSE](LICENSE) for details.

---

## 🙌 Credits

Developed by [Charitardha555](https://github.com/Charitardha555), contributors, and the Hackers Gurukul community.

---
