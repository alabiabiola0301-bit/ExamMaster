# User Flows

## Overview

This document describes how users interact with the ExamMaster platform. User flow diagrams help visualize the journey users take when performing specific actions within the system.

---

# Student Registration Flow

```mermaid
flowchart TD
    A[Visit ExamMaster] --> B[Click Register]
    B --> C[Enter Registration Details]
    C --> D[Submit Registration Form]
    D --> E[Account Created]
    E --> F[Login to Platform]
```

---

# Student Login Flow

```mermaid
flowchart TD
    A[Open Login Page] --> B[Enter Email and Password]
    B --> C{Credentials Valid?}
    C -->|Yes| D[Access Dashboard]
    C -->|No| E[Display Error Message]
    E --> B
```

---

# Student CBT Examination Flow

```mermaid
flowchart TD
    A[Login] --> B[Open Dashboard]
    B --> C[Select Subject]
    C --> D[Start CBT Test]
    D --> E[Answer Questions]
    E --> F[Navigate Between Questions]
    F --> G[Submit Examination]
    G --> H[Auto Grading]
    H --> I[View Results]
```

---

# Resource Download Flow

```mermaid
flowchart TD
    A[Login] --> B[Browse Subjects]
    B --> C[Open Subject Page]
    C --> D[View Resources]
    D --> E[Select Resource]
    E --> F[Download Resource]
```

---

# Performance Analytics Flow

```mermaid
flowchart TD
    A[Login] --> B[Open Dashboard]
    B --> C[Open Analytics Section]
    C --> D[View Score History]
    D --> E[View Subject Performance]
    E --> F[Identify Weak Areas]
```

---

# Content Manager Flow

```mermaid
flowchart TD
    A[Login] --> B[Open Content Manager Dashboard]
    B --> C[Upload Resource]
    B --> D[Create Question]
    B --> E[Edit Existing Content]
    C --> F[Save Content]
    D --> F
    E --> F
```

---

# Admin User Management Flow

```mermaid
flowchart TD
    A[Admin Login] --> B[Open Admin Dashboard]
    B --> C[View Users]
    C --> D[Select User]
    D --> E[Update Role]
    D --> F[Suspend User]
    D --> G[Delete User]
```

---

# Admin Content Management Flow

```mermaid
flowchart TD
    A[Admin Login] --> B[Open Admin Dashboard]
    B --> C[Manage Subjects]
    B --> D[Manage Resources]
    B --> E[Manage Questions]
    C --> F[Save Changes]
    D --> F
    E --> F
```

---

# Complete Student Journey

```mermaid
flowchart TD
    A[Visit Platform]
    A --> B[Register Account]
    B --> C[Login]
    C --> D[Access Dashboard]
    D --> E[Study Materials]
    D --> F[Take CBT Practice]
    F --> G[Receive Results]
    G --> H[View Analytics]
    H --> I[Improve Weak Areas]
    I --> F
```

---

# System Flow Summary

## Student

- Register
- Login
- Access Dashboard
- Study Materials
- Take CBT Exams
- View Results
- Monitor Performance

## Content Manager

- Login
- Upload Resources
- Create Questions
- Update Content

## Admin

- Login
- Manage Users
- Manage Subjects
- Manage Resources
- Manage Questions
- View Analytics