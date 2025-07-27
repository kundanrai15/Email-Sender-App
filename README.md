
# 📧 Email Sender Application

A simple web application that allows users to send emails with optional file attachments. Built using **Spring Boot** for the backend and **HTML/CSS/JavaScript** for the frontend.

---

## ✨ Features

- Send email to any valid recipient
- Add subject and message body
- Upload and attach files (PDF, DOCX, images, etc.)
- User-friendly and responsive interface
- Backend email handling using JavaMailSender

---

## 🛠️ Tech Stack

| Layer      | Technology         |
|------------|--------------------|
| Frontend   | HTML, CSS, JavaScript |
| Backend    | Java, Spring Boot  |
| Email API  | JavaMailSender     |
| Build Tool | Maven              |

---

## 📂 Project Structure

```
EmailSenderApp/
├── src/
│   └── main/
│       ├── java/
│       │   └── com.example.demo/
│       │       ├── controller/
│       │       │   └── EmailController.java
│       │       ├── service/
│       │       │   └── EmailService.java
│       │       └── EmailSenderApplication.java
│       └── resources/
│           ├── static/
│           │   ├── index.html
│           │   ├── styles.css
│           │   └── script.js
│           └── application.properties
└── pom.xml
```

---

## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/email-sender-app.git
cd email-sender-app
```

### 2. Configure SMTP in `application.properties`

```properties
spring.mail.host=smtp.gmail.com
spring.mail.port=587
spring.mail.username=your-email@gmail.com
spring.mail.password=your-app-password
spring.mail.properties.mail.smtp.auth=true
spring.mail.properties.mail.smtp.starttls.enable=true
```

> ⚠️ Use an App Password if you're using Gmail (2FA enabled accounts).

---

### 3. Run the Application

```bash
mvn spring-boot:run
```

The app will start at `http://localhost:8080`.

> Open `index.html` manually in a browser (you can place it in `resources/static` or serve with controller if needed).

---

## 🧪 API Endpoint

| Method | Endpoint           | Description        |
|--------|--------------------|--------------------|
| POST   | `/api/email/send`  | Sends email with optional file |

---

## 📸 UI Preview



---

## 🙋‍♂️ Author

**Kundan Rai**
