# Memory Compensation Application
**Capstone Project - Fall 2025**

A responsive web application developed for QLI rehabilitation center to support residents with memory challenges during their recovery journey.

## 📋 Project Overview

This application provides residents with centralized access to:
- Personal profile information and emergency contacts
- Therapist information and photos
- Automated therapy session schedules pulled from Microsoft Outlook
- Campus and building maps and photos for reference
- Shared notes system for residents and therapists to track session progress and homework

The application addresses a real-world need identified by QLI staff: helping residents with cognitive impairments maintain awareness of their therapy schedules, locations, and daily tasks.

## 🎯 Problem Statement

Residents at QLI rehabilitation center often experience memory difficulties due to traumatic brain injuries or other cognitive impairments. They need:
- Easy access to their daily therapy schedules
- Visual aids for navigating campus buildings
- A system to track therapy notes and homework assignments

Our application consolidates this information into a single, user-friendly interface accessible via Microsoft authentication.

## 👥 Team

- **Julianne Furey** - Database Architecture & Backend Development 
- **Sarah Lemi** - Project Manager & Backend Development
- **Allison Coates** - Frontend Development & UI/UX

## 🛠️ Technology Stack

**Frontend:** Vue.js  
**Backend:** Flask (Python) RESTful API  
**Database:** MySQL (hosted on DigitalOcean)  
**Authentication:** Microsoft Azure OAuth 2.0  
**External API Integration:** Microsoft Graph API (Calendar access)

## 💼 My Contributions

As a backend developer, I was responsible for:

### Database Design & Implementation
- Designed and implemented a **5-table relational database schema** with proper foreign key constraints
- Created tables for: residents, therapists, buildings, sessions, and session_notes
- Developed seed data and validation scripts for testing
- Set up cloud-hosted MySQL database on DigitalOcean for team development and testing

### Backend Development
- Built RESTful API endpoints using Flask for:
  - Therapist management (`therapists.py`)
  - Building and location data, including photo retrieval (`buildings.py`)
  - Microsoft authentication and calendar integration (`ms_auth.py`)
- Implemented comprehensive CRUD operations with proper error handling

### Microsoft Integration
- Integrated **Microsoft Graph API** for calendar event retrieval
- Implemented **OAuth 2.0 authentication flow** with Azure AD for resident login
- Built automatic **token refresh mechanism** for persistent sessions
- Created event parsing logic to filter and format therapy appointments from Outlook calendars
- Linked resident Microsoft accounts to database records via unique identifier
  
### DevOps & Deployment
- Deployed cloud-hosted MySQL database on DigitalOcean for development and testing
- Configured environment variables for secure credential storage (database, API keys)
- Organized and processed building photos provided by client

## 📊 Project Poster

![Capstone Poster](CapstonePoster_QLI004.pdf)

*Presented at University of Nebraska at Omaha Computer Science Capstone Showcase - Fall 2025*

## 🔒 Code Repository

The source code for this project is maintained in a **private repository** due to client confidentiality agreements with QLI. I'm happy to discuss the technical implementation, architecture decisions, and challenges solved during interviews.

## 🎓 Academic Context

- **Course:** CSCI 4970 - Computer Science Capstone
- **Institution:** University of Nebraska at Omaha
- **Semester:** Fall 2025
- **Client:** QLI - Omaha, Nebraska

---

*This project demonstrates real-world software development experience including client communication, agile methodology, team collaboration, and production deployment of a full-stack application.*
