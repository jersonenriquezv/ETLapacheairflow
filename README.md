# ETL Server Access Log Proccessing with Apache Airflow

From this project I have learned to work with Apache Airflow and see the proccess of the ETL pipeline.

# KEY LEARNING

### 1. Connecting my IDE and Visualizing the UI from a Local Server
### 2. Better Understanding of the ETL Process and Data Flow
    The airflow UI is so helpful and simplifies the flow, making it easier to develop, manage and monitor the process in a more interactive way. 
## 3. Challenges with Connections and Directories
    I had a challenge when trying to connect to the server. It was so simple but it was my first time working with Apache and also 
    faced some challenges navigating between files and directories using bash, which led to troubleshooting permission and path error or permissions denied 
    so sending the correct DAG folder in Airflow was tricky at first but once I understand the file structure and some debugging I could succesfully deployed my DAG

****## Technologies Used
- **Apache Airflow**: Orchestrating the ETL pipeline.
- **Python: Writing tasks for the pipeline.
- **Bash commands**
- **Git & GitHub**: Version control and code repository.
****
## Project Setup

1. **Environment Setup**: Created a Python virtual environment and installed Apache Airflow.
2. **Airflow Configuration**: Configured Airflow to run locally and tested the DAG (Directed Acyclic Graph).
3. **Python Code**: Created Python scripts to handle each stage of the ETL process:
   - `download_file()`: Downloads the log file.
   - `extract()`: Extracts the required fields.
   - `transform()`: Transforms the data by capitalizing the `visitorid`.
   - `load()`: Loads the data into `capitalized.txt`.
   - `check()`: Verifies the output.
   - ## DAG Workflow

The DAG runs a simple ETL process extranging the data from URL provided by IBM
- **Download**: Fetches the log file from the URL.
- **Extract**: Extracts the required fields.
- **Transform**: Capitalizes the `visitorid`.
- **Load**: Writes the transformed data to a file.
- **Check**: Prints the contents of the final output.


 Here are some images to overview the results
![capitalizedfile](https://github.com/user-attachments/assets/e6cd91db-08c6-49a4-a8ab-729fa1efc2ea)
![graphview](https://github.com/user-attachments/assets/aef6b847-3e17-444e-a320-dbae2dd67c1c)
![grant](https://github.com/user-attachments/assets/c55683d7-35eb-4d89-b0cd-66f0f24b3749)
![eventlog](https://github.com/user-attachments/assets/0a9d3c4d-dd37-43f0-b394-ebfe559b0b4f)
![ETLsuccess](https://github.com/user-attachments/assets/a5ca6a57-eed4-4e26-b015-1d84d2c910a0)
![dagsoverview](https://github.com/user-attachments/assets/57fbf57b-779f-41bf-b0d2-be002d3cadd8)



