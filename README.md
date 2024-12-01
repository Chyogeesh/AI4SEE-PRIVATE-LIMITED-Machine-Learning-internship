# AI4SEE-PRIVATE-LIMITED-Machine-Learning-internship
It is a Internship assignment
The code you provided is a Python script intended to collect hardware monitoring data such as CPU temperature, usage, load, memory usage, battery level, and CPU power, and store it in a CSV file. It uses the WMI library for hardware monitoring and psutil for system resource information. Additionally, it randomly introduces synthetic anomalies in the data to mimic unusual system behaviors.
Description
Data Collection:

The script collects hardware data such as CPU temperature, CPU usage, memory usage, battery level, and CPU power.
It uses WMI for hardware-related metrics and psutil for system metrics like CPU and memory usage.
Synthetic Anomalies:

Anomalies are introduced at random with a 10% probability for each metric.
Examples include unusually high CPU usage, memory usage, temperature, or low battery levels.
CSV Storage:

Data is saved incrementally to a CSV file (hardware_monitor_data.csv) every 100 samples to minimize memory usage.
Error Handling:

If any error occurs during data collection, None is appended to the respective lists, ensuring that the program continues to run.
Performance:

The program uses incremental saving and clears memory after each save to handle large datasets efficiently.
Next Steps: Anomaly Detection
Once the data is generated, apply a simple anomaly detection algorithm (e.g., Z-Score, Isolation Forest) on metrics like CPU usage or memory usage to detect outliers. Display the detected anomalies in the form of plots or tables. Let me know if you'd like help implementing anomaly detection!
