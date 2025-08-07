# 📊 SQL_Insights.Gemini.Activities

**SQL_Insights.Gemini.Activities** is a custom Automation Anywher activity that connects to a SQL Server database and retrieves analytical insights using Google Gemini API.

---

## 📦 Overview

- **Command Name:** `sqlInsightsUsingGemini`
- **Package:** `SQLInsights.commands`
- **Technology:** Java (Automation Anywhere SDK)
- **LLM Integration:** Google Gemini API
- **Database Support:** Microsoft SQL Server

---

## ✅ Features

- ✅ Accepts natural language questions and generates valid SQL Server `SELECT` queries.
- ✅ Uses the database schema to ensure valid table/column references.
- ✅ Executes the generated query via JDBC.
- ✅ Passes result data back to Gemini to get a clean, natural-language insight.
- ✅ Returns the final insight (or a no-result message).

---

## 🧾 Inputs

| Parameter           | Type   | Required | Description                                          |
|---------------------|--------|----------|------------------------------------------------------|
| `Connection String` | Text   | ✅        | JDBC connection string for SQL Server               |
| `Gemini API Key`    | Text   | ✅        | Your Google Gemini API key                          |
| `Gemini Model`      | Text   | ✅        | The Gemini model to use (e.g., `gemini-pro`)        |
| `User Prompt`       | Text   | ✅        | A natural language request (e.g., "Top 5 customers") |

---

## 📤 Outputs

| Name     | Type   | Description                                     |
|----------|--------|-------------------------------------------------|
| Response | String | Gemini's response with insight or summarized data.|

---

## ⚙️ Dependencies

- Java 11+
- Automation Anywhere SDK
- Microsoft SQL Server JDBC Driver
- Google Gemini API access and valid API key


> 🧱 **Native Dependency Note**: Connection String:
> `jdbc:sqlserver://HOST;databaseName=YOUR_DATABASE;user=YOUR_USERNAME;password=YOUR_PASSWORD;trustServerCertificate=true;`

---

## 💡 Use Cases

- Business analysts or users can ask questions about databases without writing SQL.
- Generate reports or summaries from live data with Gemini.
- Automate insight generation from structured data.

---

## 🔧 How to Install

1. Download the `.nupkg` file from the [Releases](https://github.com/AmrEzzatAbdo/SQL_Insights.Gemini.Activities-_AA/releases/).
2. Move to packages and upload the package.

---

## 📜 License

This project is licensed under the [MIT License].

---

## 👨‍💻 Author

Developed by **Amr Ezzat**

- LinkedIn: [linkedin.com/in/amr-ezzat](https://www.linkedin.com/in/amrezzatabdal-al/)
- Email: `amrezzat289@gmail.com`

---

> Feel free to contribute or open issues for improvements!
