# Agentic AI Customer Support Orchestrator

## Overview
This project implements a "Hub-and-Spoke" agentic AI system using n8n. It simulates a technical support team with a central Controller Agent routing issues to specialized experts (Python Backend vs. General Support).

## Features
- **Controller Agent:** Analyzes user intent to route tickets without solving them.
- **Custom Tool (`clean_log_tool`):** JavaScript-based tool to sanitize raw server logs by removing timestamps.
- **Specialized Workflows:**
  - **Python Expert:** Fixes API/Backend code.
  - **General Assistant:** Handles operational queries using Wikipedia and Time tools.

## Prerequisites
- n8n (Self-hosted or Cloud) v1.0+
- Groq API Key (for Llama-3.3-70b model)

## Setup Instructions
1. Import `DevSupport_Orchestrator_Workflow.json` into n8n.
2. Set up your Groq Credentials in n8n.
3. Activate the workflow or use the "Test Workflow" button.

## Usage
- **Python Debugging:** Type "I have a Python error: [logs]"
- **General Info:** Type "What time is it?"

<img width="460" height="374" alt="image" src="https://github.com/user-attachments/assets/a276716a-7f4e-4475-b0f4-187a46bb22c6" />
