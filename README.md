# Hi there 👋  
Welcome to my workspace 🚀  

I build automation tools, browser workflows and productivity-focused applications.  
This repository contains my daily work environment and utilities.

---

## ⚙️ Environment setup

Activate the virtual environment (Windows):

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope Process
.\.venv\Scripts\Activate.ps1
```

>[!TIP]
>If you want to avoid running this every time:
>
>```powershell
>  Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
>```

---

## 🔐 Security & Git hygiene

To prevent accidentally committing sensitive files
(credentials, configs, local state, etc.), you can tell Git to ignore changes:

```powershell
git update-index --assume-unchanged "File/Path/Name"
```

This is especially useful for:

- `config.json`

- local environment files

- temporary credentials

---

## 🚀 Featured projects

Here are some projects I actively maintain or use as foundations:

### 🧭 Browser Automation

Declarative browser automation using JSON flows and Selenium.

**👉 Repository:**\
🔗 [browser-automation](https://github.com/LJD-UwU/browser-automation "Ir a ver")

**Highlights:**

- JSON-based workflows

- Automatic Edge driver handling

- Stable downloads

- Windows & Linux support

### ✂️ Recort App

A lightweight tool focused on productivity and utility workflows.

**👉 Repository:**\
🔗 [Recort_app](https://github.com/LJD-UwU/Recort_app "Ir a ver")

---

## 🧠 What I focus on

- Browser automation

- Workflow optimization

- Clean architecture

- Reusable tooling

- Developer experience

I prefer simple, explicit systems that scale without becoming fragile.
