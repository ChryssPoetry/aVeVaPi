# aVeVaPi
### Comprehensive Documentation for Sensor Monitoring and Analytics Project

#### **1. Project Overview**
The project involves creating a real-time sensor monitoring system using simulated data. This system demonstrates the integration of Python-generated data with analytical tools and visualizations, such as PI Vision, to monitor industrial equipment.

---

2. Architecture Diagram**

**Components:**
- **Data Generator:** Python script generates sensor data (temperature, pressure, humidity).
- **Data Storage:** CSV file stores the simulated data.
- **Data Processing:** Python cleans and processes the data.
- **Integration:** PI System (e.g., PI AF, PI Vision) for real-time monitoring.
- **Visualization:** PI Vision for dashboard creation.

**Workflow:**
1. Python generates simulated sensor data and stores it in a CSV file.
2. The CSV file is ingested by PI System using PI UFL or similar interfaces.
3. Data is structured in PI AF with calculated attributes.
4. PI Vision displays dashboards for real-time and historical analysis.

---

### **3. Step-by-Step Setup Instructions**

#### **A. Data Generation**
1. Run the Python script to generate sensor data:
   ```python
   python generate_sensor_data.py
   ```
2. Verify that the data is being stored in `sensor_data.csv`.

#### **B. Data Preprocessing**
1. Use the provided preprocessing script to clean the data:
   ```python
   python clean_sensor_data.py
   ```
2. Confirm that `cleaned_sensor_data.csv` is created.

#### **C. Integration with PI System**
1. Configure PI Points for `temperature`, `pressure`, and `humidity`.
2. Use PI UFL to import the cleaned data into the PI Server.
3. Create an Asset Framework (AF) template:
   - Add attributes for temperature, pressure, and humidity.
   - Map attributes to the respective PI Points.

#### **D. Visualization in PI Vision**
1. Log in to PI Vision.
2. Create a new dashboard:
   - Add trends for temperature, pressure, and humidity.
   - Configure thresholds to highlight anomalies.
3. Save the dashboard and verify real-time updates.

---

### **4. Screenshots**

#### **A. Python Results**
- **Data Generation:**
  ![Python Data Generation](#)
- **Cleaned Data:**
  ![Cleaned CSV Data](#)

#### **B. PI Vision Dashboards**
- **Real-Time Trends:**
  ![Real-Time Dashboard](#)
- **Threshold Alerts:**
  ![Alerts and Notifications](#)

### **5. Real-World Applications**

#### **Industrial Equipment Monitoring**
- Real-time data tracking for machinery to predict failures and reduce downtime.
- Use thresholds to trigger maintenance alerts.

#### **Process Optimization**
- Analyze historical data to identify inefficiencies in industrial processes.
- Optimize resource allocation and energy usage.

#### **Predictive Maintenance**
- Use analytics to predict equipment failures based on trends.
- Schedule proactive maintenance to extend equipment life.

### **6. Conclusion**
This project showcases the integration of Python-generated data with advanced visualization and monitoring tools like PI Vision. The system demonstrates the potential for real-world industrial applications, including enhanced efficiency, reduced downtime, and improved decision-making.



