
# 🖥️ Batch Operating System

This project is a **Batch Operating System Simulator** designed to handle batch processing jobs. It reads job descriptions from input files, processes these jobs, and produces output files detailing the results. The system simulates job scheduling, processing, and reporting.

---

## 🛠️ Features

- **Job Processing**: Handles batch job commands and processes them sequentially.
- **Job Status Reporting**: Provides detailed status reports and error messages.
- **Input/Output Handling**: Reads from input files and writes results to output files.
- **Error Handling**: Includes mechanisms for managing time limits and abnormal terminations.

---

## 📂 Project Structure

```
batch-os-simulator/
│
├── src/
│   ├── BatchJobProcessor.java  # Core logic for processing batch jobs
│   ├── JobScheduler.java       # Manages job scheduling and execution
│   ├── ReportGenerator.java    # Generates status and error reports
│   └── Main.java               # Entry point for the application
├── input.txt                   # Example input file
├── output.txt                  # Example output file
├── README.md                   # Instructions (this file)
└── build.gradle                # Gradle build script
```

---

## 🚀 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/Aniketpagare1/Batch-Operating-System.git
cd Batch-Operating-System
```

### 2. Build the Project

Ensure you have Gradle installed. Build the project using:

```bash
gradle build
```

### 3. Run the Application

Execute the application using:

```bash
gradle run
```

You should see output indicating the job processing status.

---

## 🛠️ Usage

### **Input Format**

- **Job Description**: Jobs are defined in an input file with specific commands and data.
- **Example Input File** (`input.txt`):
  ```txt
  // Sample job description
  $AMJ020200120005
  GD20PD20LR20SR30SR31PD30SR40SR41SR42PD40
  PD30PD20H
  $DTA
  *
  $END0202
  ```

### **Output Format**

- **Job Results**: Results and status reports are generated and saved in an output file.
- **Example Output File** (`output.txt`):
  ```txt
  *
  **
  ***
  **
  3: Time limit exceeded. Program terminated abnormally.
  SI: 2 PI: 0 TI: 2 TTC: 13 LLC: 5
  ```

---

## 🔑 Notes

- **Time Limits**: Ensure jobs complete within specified time limits to avoid abnormal termination.
- **Error Handling**: The system will generate detailed error messages for any issues encountered during job processing.

---

