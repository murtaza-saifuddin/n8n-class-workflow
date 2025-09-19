# n8n Class Workflow

This repository contains an **automated n8n workflow** created as part of a class project.  
The workflow demonstrates process automation by combining scheduling, API integration, database storage, and team communication.

---

## About the Project
This project showcases an n8n workflow developed to demonstrate **end-to-end automation**.  

The workflow executes on a scheduled trigger, retrieves order data through an API, and applies conditional logic to filter relevant records. Filtered orders are stored in Airtable for structured management. A JavaScript code node is used to aggregate data, calculating the total number of booked orders and their combined value. Finally, a summary report is sent to a Discord channel for team visibility.  

This project highlights the flexibility of n8n in building no-code/low-code automation pipelines, combining multiple services into a single workflow. It serves as a practical example of how repetitive tasks can be streamlined, collaboration improved, and reporting automated.  

---

##  Workflow Overview
- **Trigger:** Runs weekly on Monday at 9 AM  
- **HTTP Request:** Fetches order data from an external API  
- **If Condition:** Filters only the orders with status = `processing`  
- **Set Node:** Extracts `orderID` and `employeeName`  
- **Airtable:** Stores the filtered records in Airtable for tracking  
- **Code Node (JavaScript):** Calculates the total number of booked orders and their sum  
- **Discord:** Sends a weekly summary report to a Discord channel  



##  Workflow Screenshot
![Workflow Screenshot](workflow-screenshot.png)<img width="1360" height="685" alt="{4F2F503E-E7FD-4E47-AD4C-61DF4F8DA5B6}" src="https://github.com/user-attachments/assets/2bf7a461-3cb6-4ca9-b1eb-cd9e5949070d" />




##  Files
- `class-n8n-workflow.json` → The exported workflow  
- `workflow-screenshot.png` → Visual representation of the workflow
  
  

 **Purpose:**  
Demonstrates automation, database integration, and reporting using n8n.  


