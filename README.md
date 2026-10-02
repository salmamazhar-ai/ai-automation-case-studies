# 📧 Automated Student Assignment Submission Notification System

A no-code workflow that sends every student an instant confirmation 
email the moment an assignment is submitted — built with Zapier, 
Google Forms, Google Sheets, and Gmail.

---

## 📋 Overview

| | |
|---|---|
| **Role** | Workflow Automation Designer |
| **Platform** | Zapier (No-Code Automation) |
| **Tools Used** | Zapier · Google Forms · Google Sheets · Gmail · Miro |
| **Domain** | Education Technology |

## 🎯 The Challenge

In any classroom or tutoring practice, a student who submits work 
wants one thing straight away: proof that it arrived. Without it, 
students ask "Did you get my file?", teachers answer the same message 
repeatedly, and some work is wrongly reported as missing.

**Teacher side:** Repeated confirmation emails, hard-to-track 
submissions, and time taken away from feedback and planning.

**Student side:** Uncertainty after submitting, delayed replies, and 
no record to point to if a dispute comes up.

## 💡 The Goal

Design a simple, reliable process where every submission is recorded 
automatically and every student gets a confirmation within moments, 
using free or low-cost tools that any teacher can maintain without 
writing code.

## 🗺️ Planning the Idea

Before opening Zapier, I mapped the project on a Miro board: the 
problem, the step-by-step workflow, the value for teachers and 
students, target users, and the expected outcome. Starting with a 
clear flowchart kept the build small and focused.

## 🛠️ How It Works
Google Form → Google Sheets → Zapier → Gmail
(Student (Row is (Detects (Sends
submits) stored) new row) confirmation)
Each response is saved as a row in Google Sheets. Zapier watches that 
sheet and tells Gmail to email the address the student entered, so 
the confirmation only goes out after the submission is safely stored.

### Step 1: Collect Submissions (Google Forms + Sheets)
The Student Assignment Submission Form asks for name, email, 
assignment title, course name, submission date, and an assignment 
link. Required fields keep the data complete, and the form tells 
students up front that a confirmation will follow.

### Step 2: Set the Trigger (Zapier)
The first step of the Zap uses the "New Spreadsheet Row" trigger — 
connected to the Google account, the responses spreadsheet, and the 
"Form responses" worksheet, tested to confirm Zapier could pull a 
real sample record.

**Design Decision:** Triggering from the sheet, not from the form, 
means the email only fires after the response has been safely stored. 
If something fails, the data is never lost.

### Step 3: Send the Confirmation (Gmail)
The second step sends the email. The recipient field is mapped 
dynamically to the Student Email column, so every message goes to 
the person who submitted. The subject, "Assignment Submitted 
Successfully!", gives the outcome before the student even opens it.

### Step 4: Publish and Verify
After publishing the Zap, I submitted several test responses and 
checked three places: the Zap run history, the response sheet, and 
the Gmail sent folder.

**Results:**
- ✔️ 4 test submissions recorded
- ✔️ 3 confirmation emails delivered
- ✔️ 1 successful Zap run logged

## 📚 Lessons Learned

**Start from the user's worry**
The product answers one question: "Did my work arrive?" Naming that 
moment early kept the scope small.

**Clean data makes reliable automation**
The email depends on the Student Email column, so required form 
fields are part of system reliability.

**Test with real records**
Sample rows from the actual sheet exposed mapping mistakes a mock-up 
would have hidden.

## 🚀 Next Improvements

- **Personalize the message** — Add student name, assignment title, 
  and submission time
- **Notify the teacher** — Send a daily digest of new submissions
- **Handle late work** — Compare the date with a deadline and use a 
  different message
- **Add a safety net** — Alert the teacher if an email fails or an 
  address is invalid

## 🎓 Skills Demonstrated

`Workflow Automation` `No-Code Tools (Zapier)` `Process Mapping (Miro)` 
`System Design` `Google Workspace Integration` `Testing & Verification` 
`Education Technology`

---

## 🤝 Let's Connect

Need a workflow like this for your classroom or business? I design 
automations that save you time — from mapping the problem to a 
tested, working system.

**Built by [Salma Mazhar](https://www.linkedin.com/in/salma-mazhar)**
