# N8N Agentic AI Booking System

An AI-powered conversational booking automation workflow built using **N8N**, **Agentic AI**, **RAG Architecture**, and **Google Workspace APIs**.
This system can intelligently interact with users, retrieve company information from a Vector Database, and automatically schedule meetings without human intervention.

---

# Project Overview

This project demonstrates how **AI Agents**, **Retrieval-Augmented Generation (RAG)**, and workflow automation can be combined to build a real-world business assistant.

The workflow consists of:

* A Main Conversational AI Agent
* A Company Knowledge Retrieval System
* A Dedicated Booking Agent
* Google Calendar Integration
* Automated Email Confirmation System
* Memory-Based Conversation Handling

The entire workflow is orchestrated inside **N8N**.

---

# Features

## AI Conversational Agent

* Handles natural language conversations
* Understands user queries
* Maintains conversation memory
* Routes requests intelligently

## RAG-Based Knowledge Retrieval

* Retrieves company information from:

  * Supabase Vector Database
  * Google Docs
* Uses semantic search with embeddings
* Provides contextual responses

## Dedicated Booking Agent

* Activated when user requests a meeting
* Collects:

  * Name
  * Email
  * Meeting Topic
  * Date
  * Time

## Google Calendar Automation

* Checks calendar availability
* Prevents scheduling conflicts
* Automatically creates calendar events

## Email Notification System

* Sends confirmation emails to:

  * User
  * Internal Team
* Includes meeting details automatically

## Multi-Agent Workflow

* Main AI Agent handles conversations
* Booking Agent handles scheduling tasks
* Agents communicate dynamically

---

# Workflow Architecture

User → Main AI Agent → Knowledge Retrieval (RAG)

If Booking Required:

Main AI Agent → Booking Agent → Google Calendar → Gmail Confirmation

---

# Tech Stack

## Automation

* N8N

## AI & LLMs

* Google Gemini
* Groq LLM

## Embeddings

* HuggingFace Embeddings

## Vector Database

* Supabase Vector Store

## APIs & Services

* Google Calendar API
* Gmail API
* Google Docs API

## AI Concepts Used

* Agentic AI
* Multi-Agent Systems
* RAG (Retrieval-Augmented Generation)
* Conversational Memory
* Semantic Search

---

# Workflow Components

## Main AI Agent

Responsible for:

* User interaction
* Context understanding
* Query routing
* Knowledge retrieval

## Memory System

Stores previous conversation context to improve user interaction.

## Supabase Vector Database

Stores embedded company knowledge for semantic retrieval.

## Google Docs Integration

Used as an additional company knowledge source.

## Booking Agent

Handles:

* Appointment booking
* Calendar availability
* Meeting scheduling
* Confirmation process

## Gmail Notification System

Automatically sends:

* Booking confirmations
* Team notifications

---

# Use Cases

* AI Customer Support
* Automated Appointment Booking
* Business Information Assistant
* AI Receptionist
* Company Helpdesk Automation
* Conversational Business Assistant

---

# Installation & Setup

## Clone Repository

```bash
git clone https://github.com/Ali-Zia3500/n8n-agentic-booking-system.git
cd n8n-agentic-ai-booking-system
```

---

# Required Services

Create accounts and configure APIs for:

* N8N
* Google Cloud Console
* Supabase
* Groq
* Google Gemini
* HuggingFace

---

# Environment Variables

Create a `.env` file and add:

```env
GEMINI_API_KEY=your_api_key
GROQ_API_KEY=your_api_key
SUPABASE_URL=your_url
SUPABASE_API_KEY=your_key
GOOGLE_CLIENT_ID=your_client_id
GOOGLE_CLIENT_SECRET=your_secret
GOOGLE_REFRESH_TOKEN=your_token
```

---

# Import Workflow into N8N

1. Open N8N
2. Click "Import Workflow"
3. Upload workflow JSON file
4. Configure credentials
5. Activate workflow

---

# How the System Works

## Step 1

User sends a message to the AI Agent.

## Step 2

The Main Agent:

* Understands the query
* Retrieves company information using RAG
* Responds intelligently

## Step 3

If user requests a meeting:

* Booking Agent is activated
* Collects booking details

## Step 4

Booking Agent:

* Checks Google Calendar availability
* Creates event automatically

## Step 5

System sends confirmation emails to:

* User
* Team Members

---

# Future Improvements

* WhatsApp Integration
* Telegram Bot Support
* Voice-Based AI Agent
* CRM Integration
* Multi-Language Support
* Human Handoff System
* Analytics Dashboard

---

# Learning Outcomes

This project helped in understanding:

* Agentic AI Systems
* Multi-Agent Workflows
* RAG Architecture
* AI Automation
* Vector Databases
* Conversational AI
* Workflow Orchestration
* API Integrations

---

# Author

Ali Zia

AI Engineer | Generative AI Developer | Agentic AI Enthusiast

---

# License

This project is licensed under the MIT License.

---
