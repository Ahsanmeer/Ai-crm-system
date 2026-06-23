🤖 AI-Powered CRM System

An intelligent CRM automation built with n8n, OpenAI, Google Sheets, and Gmail — designed to automatically capture leads, qualify them with AI, send personalized emails, and update your CRM records without any manual work.


✨ What It Does


Captures Leads — A webhook receives incoming lead data from any source (forms, apps, APIs)
AI Qualification — An AI Agent (powered by OpenAI) analyzes and qualifies the lead
Parses & Structures Data — Extracts clean, structured data from the AI response
Logs to Google Sheets — Automatically appends the lead to your CRM spreadsheet
Sends Personalized Email — Fires a tailored follow-up email via Gmail
AI Follow-up Logic — A second LLM chain decides the next best action
Updates CRM Row — Marks the lead status and updates the record automatically



🛠️ Tech Stack

ToolPurposen8nWorkflow automation engineOpenAIAI lead qualification & response generationGoogle GeminiAdditional AI chat modelGoogle SheetsCRM data storageGmailAutomated email sendingJavaScriptCustom data transformation logic


🔄 Workflow Architecture

Webhook → AI Agent → Parse Output → Google Sheets
                ↓                        ↓
         OpenAI Chat Model         Basic LLM Chain 1
                                         ↓
                                    Send Gmail
                                         ↓
                                  Basic LLM Chain 2
                                         ↓
                              JavaScript Transform
                                         ↓
                                  Update CRM Ro
