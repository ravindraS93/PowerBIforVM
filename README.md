
![Copy of Copy of Deploy-MDATP-for-Linux-using-Ansible](https://github.com/user-attachments/assets/d4e55d31-2f6b-479c-ac4c-2cc43912b3d8)

**Before we proceed, I'd like to clarify a few points:**

1. The data used for demonstration purposes is dummy data created solely for reference. It bears no relation to any actual corporate environments.
2. I'm not an expert in Power BI, but I do have some basic knowledge based on my day-to-day experience.
3. ChatGPT was used to generate the code for each task and then all this code is reviewed, modified and combined as per my requirement to attain the desired result.

Hi All,

I'm Ravi, a Cyber Security Professional with over 6 years of experience in implementing and managing cybersecurity tools. Anyone working in the IT industry, or any industry for that matter, can relate to how tedious it is to build reports every month and how crucial these reports are in showcasing the efforts being put in.

Based on my recent experience with vulnerability management, reporting has been crucial in providing insights on the following topics:
1. Displaying the current vulnerability posture of the environment
2. Tracking the inflow of new vulnerabilities
3. Measuring the rate at which vulnerabilities are being remediated
4. Identifying the major contributors to critical vulnerabilities

**NOTE**

The base data we are taking for building this dashboard is being taken from the custom report we built using python. Reference: https://github.com/ravindraS93/ExcelwithPython

**UseCase**

Here are some key metrics that are essential for comprehensive vulnerability reporting:
1. **Count of detected vs fixed vulnerabilities per month**: This helps in understanding the remediation efforts and their effectiveness over time.
2. **Trend of inflow based on severity**: Analyzing the severity of incoming vulnerabilities to prioritize remediation efforts.
3. **Count of vulnerabilities with and without exploits**: Differentiating between vulnerabilities that have known exploits and those that do not, to assess the risk level.
4. **Count of assets assessed based on environment**: Tracking the number of assets evaluated in different environments (e.g., production, development) to ensure comprehensive coverage.
5. **Summary of vulnerabilities per OS platform**: Providing an overview of vulnerabilities categorized by operating system platforms to identify platform-specific risks.

These metrics provide a holistic view of the vulnerability landscape and help in making informed decisions to enhance security posture.

**What did we do?**

Power BI is indeed a vast topic, but here's a simple explanation of the steps taken to visualize the data:

1. **Created a Date Table**: Using Power Query, a Date Table was created with columns for week number, month, and year.
2. **Merged the Date Table with the Detection Table**: The Date column in the Date Table was mapped to the First Detected and Actual Fixed Date columns in the Detection Table.
3. **Grouped the Rows by Date and Severity**: The data was grouped by date and severity to organize the information effectively.
4. **Created Count for Matching Dates Based on Severity**: Counts were calculated for matching dates, categorized by severity.
5. **Created Required Measures**: Various measures were created from the merged data to facilitate detailed analysis and visualization.

These steps helped in transforming raw data into meaningful insights, making it easier to understand and act upon the vulnerability landscape.

**How to see the Dashboard?**
1. Download the .PBIX file
2. Install Power BI Desktop
3. Open the .PBIX file

Below is how the Dashboard looks like

![WhatsApp Image 2024-08-07 at 20 25 00_6dc187f9](https://github.com/user-attachments/assets/2593d71e-888b-4753-a6e7-1e95aa6c5500)

