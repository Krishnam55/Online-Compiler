# ByteSmith : Intelligent Coding Learning Platform

> **This is still under development.**

---

## What is ByteSmith?

**ByteSmith** is a revolutionary coding learning platform built to empower teachers and inspire students in their programming journey. It's not just a learning platform – it's an **intelligent, interactive, and adaptive environment** designed for the future of coding education.

Whether you're a teacher creating assignments or a student practicing your skills, ByteSmith transforms the traditional learning model with **AI-driven features** and **real-time coding tools**.

---

## Key Features

- **Dynamic Coding Assignments**

    - Teachers can post assignments containing **bundles of coding questions** tailored to different skill levels.
    - Students can attempt, track, and submit solutions seamlessly.

- **Smart Progress Tracker**

    - Visual dashboards help students monitor their progress and areas for improvement.
    - Teachers gain insights into class-wide performance trends in real time.

- **Powerful Online Judge**

    - Submit solutions and get instant feedback.
    - Each submission is tested against **public** and **hidden test cases**, ensuring solutions are not just correct but robust.

- **Integrated Multi-Language Online Compiler**

    - Supports multiple programming languages out of the box.
    - Run, debug, and test code instantly without leaving the platform.

- **AI Superpowers**
    - **Auto Test Case Generation**: Teachers can instantly create diverse and challenging test cases with AI assistance.
    - **Error Explainer**: Students get AI-powered, beginner-friendly explanations for errors in their code.
    - **Adaptive Learning Tools**: Personalized recommendations and hints to guide students step by step.

---

## Why ByteSmith?

This isn't about just solving problems.  
It's about:

Making **coding education smarter**.  
Providing **teachers with superpowers** to create, evaluate, and guide effortlessly.  
Giving **students an environment to experiment, fail safely, and learn fast**.

We are building the **future of coding education** – one where **AI and human creativity work together**.

---

## Tech Highlights

- **Frontend:** React.js with modern design system
- **Backend:** Node.js + Express
- **Database:** MongoDB
- **AI Engine:** Gemini API
- **Cloud Deployment:** AWS
- **Design:** TailwindCSS with custom ByteSmith theme

---

## Design Philosophy

ByteSmith features a **modern, clean, and intuitive design** that prioritizes:

- **Accessibility**: Easy to use for all skill levels
- **Performance**: Fast and responsive interface
- **Scalability**: Built to grow with your needs
- **Beauty**: Visually appealing and professional

---

## Ready to Forge Your Coding Future?

Stay tuned.  
This isn't just another coding platform.  
It's **your AI teaching assistant. Your error debugger. Your smart compiler. Your coding buddy.**

**For teachers. For students. For the future.**

---

## Environment Setup

For detailed setup instructions with conda environment, see [CONDA_SETUP.md](./CONDA_SETUP.md)

### Quick Start
```bash
# Activate environment
./setup_env.sh activate

# Start all services
./setup_env.sh start
```

Visit **http://localhost:5173** to access ByteSmith!

---

## 👨‍💼 Admin User Management

### Making a User an Admin

1. **Using the makeAdmin script (Recommended)**
   ```bash
   node scripts/makeAdmin.js user@example.com
   ```
   Replace `user@example.com` with the target user's email.

2. **Verifying Admin Status**
   ```bash
   # List all users and their admin status
   node scripts/listUsers.js
   
   # Check a specific user
   node scripts/listUsers.js | grep -A 3 "user@example.com"
   ```

### Default Admin Account
- Email: `admin@example.com`
- Password: Set during first-time setup

### Security Notes
- Keep admin privileges limited to trusted users only
- Regularly review admin users with `node scripts/listUsers.js`
- Never share admin credentials
- Use strong, unique passwords for admin accounts

---

## **How to Fix**

1. **Open `frontend/src/pages/Compiler.jsx`**
2. Make sure the last line is:
   ```js
   export default Compiler;
   ```
   and not just `export { Compiler };` or missing entirely.

---
