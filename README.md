# 🐾 Vee Assist – Home Pet Grooming

A simple, responsive static landing page for **Vee Assist**, offering doorstep pet grooming services in Amanora, Hadapsar, Pune.

Customers can explore grooming services, view pricing, and submit appointment requests through an online booking form.

## 🌐 Overview

Vee Assist provides convenient home pet grooming services, including bathing and haircuts, without requiring customers to travel to a grooming salon.

### Services & Pricing

| Service | Price |
|---|---:|
| Bath | ₹800 |
| Haircut | ₹1,600 |
| Bath + Haircut | ₹2,000 |

**Service Area:** Amanora, Hadapsar  
**Operating Hours:** 10:00 AM – 8:00 PM

## ✨ Features

- Responsive and mobile-friendly design.
- Simple and accessible user interface.
- Service descriptions and transparent pricing.
- Online appointment request form.
- Customer and pet information collection.
- Appointment date and time selection.
- Home address collection.
- Email notifications through FormSubmit.
- Client-side form validation.
- Booking submission success/error messages.
- No traditional backend or database required.

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| HTML5 | Website structure |
| CSS3 | Styling and responsive layout |
| JavaScript | Form handling and interactions |
| FormSubmit | Form processing and email notifications |
| Surge.sh | Static website hosting |
| GitHub | Source code management |

## 📁 Project Structure

```text
vee-assist/
│
├── index.html
└── README.md
```

## 📬 Booking Form & Email Notifications

The website uses [FormSubmit](https://formsubmit.co/) to process booking requests and forward them to the business email address.

### How It Works

1. A customer visits the website.
2. The customer fills in the booking form.
3. JavaScript collects the form information.
4. The browser sends an HTTP POST request to FormSubmit.
5. FormSubmit processes the submission.
6. Booking details are delivered to the configured email inbox.

### Email Configuration

Inside `index.html`, locate:

```javascript
var LEAD_EMAIL = "YOUR_EMAIL_HERE";
```

Replace it with your receiving email address:

```javascript
var LEAD_EMAIL = "yourbusiness@gmail.com";
```

**Important:** The receiving email must be activated through FormSubmit before normal email delivery.

The website uses AJAX submission to display feedback without redirecting customers.

## 💻 Run Locally

### Prerequisites

- A modern web browser.
- Python or VS Code with Live Server.

### Option 1: Python HTTP Server

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/vee-assist.git
```

Navigate into the project:

```bash
cd vee-assist
```

Start a local server:

```bash
python -m http.server 8000
```

Open:

```text
http://localhost:8000
```

### Option 2: VS Code Live Server

1. Open the project folder in VS Code.
2. Install the Live Server extension.
3. Right-click `index.html`.
4. Select **Open with Live Server**.

Note: Using a local HTTP server is preferable to opening the HTML directly through `file://`.

## 🚀 Deployment on Surge.sh

Vee Assist is a static website and can be deployed directly to Surge.sh.

### Step 1: Install Surge

```bash
npm install --global surge
```

### Step 2: Navigate to the project

```bash
cd vee-assist
```

### Step 3: Deploy

```bash
surge . veeassist.surge.sh
```

Replace the domain with your preferred available Surge subdomain.

Your website will be publicly accessible after successful deployment.

## 🔒 Privacy & Security

- Customer details are submitted to FormSubmit for email processing.
- No customer database is maintained by this website.
- Do not store passwords, API secrets, or private credentials in frontend code.
- Protect access to the receiving business email account.
- Provide an appropriate privacy notice explaining how customer information is used.

## ⚠️ Current Limitations

- Booking requests are not automatically confirmed appointments.
- No real-time appointment availability checking.
- No automatic prevention of duplicate bookings.
- No customer login or registration.
- No booking history or admin dashboard.
- Email delivery depends on FormSubmit availability and its service limits.

## 🔮 Future Improvements

- WhatsApp booking confirmation.
- Automated customer confirmation emails.
- Google Sheets booking records.
- Admin dashboard for managing requests.
- Appointment availability management.
- Customer reviews and testimonials.

## 📄 License

No open-source license is currently assigned.

All rights reserved unless otherwise specified.

## ❤️ Acknowledgements

- [Surge.sh](https://surge.sh/) – Static website hosting.
- [FormSubmit](https://formsubmit.co/) – Contact and booking form processing.
- [Google Fonts](https://fonts.google.com/) – Typography.

---

**Vee Assist** – Spa day for your pet, at your front door. 🐶

