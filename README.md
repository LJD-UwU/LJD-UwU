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

## Copiar archivos de ramas a main

Supón:

- Rama: feature/macros
- Carpeta: macro/

Entonces:

```powershell
git checkout main
git pull
git checkout feature/macros -- macro/
git add macro/
git commit -m "Import macro folder from feature/macros"
git push
```

Qué pasa exactamente

Git toma el contenido actual de:

> feature/macros:macro/

y lo copia dentro de:

> main:macro/

Como si hubieras pegado la carpeta manualmente.

**Importante**

Si en main ya existe macro/:

Los archivos iguales se sobrescriben\
Los nuevos se agregan\
Los que no existan en la rama NO se eliminan automáticamente\

**Alternativa moderna (git restore)\**
Más nuevo y limpio:

```powershell
git restore --source feature/macros -- macro/
```

Hace prácticamente lo mismo.

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
