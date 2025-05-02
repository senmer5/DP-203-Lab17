# DP-203-Lab17
# Get Started with Azure Stream Analytics

## 🌟 Objective

The purpose of this lab is to learn how to process real-time streaming data using Azure Stream Analytics. This includes capturing event data, running real-time queries, and storing the results in Azure Blob Storage for later analysis.

## 🧪 What This Lab Does

This lab simulates a sales scenario where a stream of sales transaction events is generated and processed in real time. Here’s what was done in this lab:

1. **Provision Resources**  
   - A resource group, Event Hubs namespace, and a Storage account were automatically created using a PowerShell script and ARM template in Azure Cloud Shell.

2. **Stream Real-Time Sales Data**  
   - A Node.js client was run to send 1000 simulated sales order events (including product ID and quantity) to the Event Hub.

3. **Create a Stream Analytics Job**  
   - An Azure Stream Analytics job named `process-orders` was created.
   - It was configured to:
     - Receive input from the Event Hub (`orders`)
     - Send output to Azure Blob Storage (`blobstore`)
     - Process data in 10-second tumbling windows

4. **Write and Run a Query**  
   - A query was written to:
     - Group incoming sales data by ProductID
     - Calculate the total quantity sold every 10 seconds
     - Save the results in JSON format to Azure Blob Storage

5. **Run the Job & Validate the Output**  
   - The Stream Analytics job was started and the client re-run to send new events.
   - The output JSON files were found in the storage container, showing the aggregated order data.

## 📘 Why This Lab Is Important

This lab provides hands-on experience with:

- Event-driven architecture in Azure
- Real-time data processing
- Using Stream Analytics to write temporal SQL-like queries
- Integrating Azure Event Hubs with Blob Storage for end-to-end stream processing

## 🚀 What I Learned

- How to set up a complete real-time data pipeline using Azure tools
- How to send and process event data with Event Hubs and Stream Analytics
- How to use windowing functions (like `TumblingWindow`) to aggregate data over time
- How to output query results into Azure Blob Storage in structured JSON format
- The role of managed identities in securing access between Azure services

This lab helped me understand the core concepts behind Azure Stream Analytics and how it can be used in real-world scenarios for real-time analytics and monitoring.

## screenshot

<img width="720" alt="1" src="https://github.com/user-attachments/assets/a52d4dd5-da44-4073-988c-7bc06c2226ed" />

<img width="777" alt="2" src="https://github.com/user-attachments/assets/d7cf0fbf-31b0-4735-abbf-abf7c249e67c" />

<img width="351" alt="3" src="https://github.com/user-attachments/assets/672a8d22-476b-42dd-8308-e968de17936c" />

<img width="1504" alt="4" src="https://github.com/user-attachments/assets/8d0085c2-9f29-428a-bd6d-0733fc5e5dc2" />

<img width="1502" alt="5" src="https://github.com/user-attachments/assets/87fa0501-85f1-40cf-adef-2b113a322265" />

<img width="1023" alt="6" src="https://github.com/user-attachments/assets/96ffadbb-5c60-441d-9a2c-907a6d504536" />

<img width="765" alt="7" src="https://github.com/user-attachments/assets/07aefab9-a467-4315-bbc7-ed395438c63e" />

<img width="1497" alt="8" src="https://github.com/user-attachments/assets/32b20f54-8485-4aec-ad88-6e78b320abf5" />




