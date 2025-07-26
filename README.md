Planetary Orbit Anomaly Detection
Overview
This project uses Chart.js to visualize planetary orbit data and detect anomalies in orbital distances. Anomalies are identified as data points that deviate more than 2 standard deviations from the mean orbital distance. The visualization is a scatter plot, with anomalies highlighted in red, and a list of detected anomalies is displayed below the chart.
Features

Visualization: Scatter plot of orbital distances over time using Chart.js.
Anomaly Detection: Identifies outliers using a statistical threshold (2 standard deviations).
Interactive: Hover over data points to see their values and anomaly status.
Responsive Design: Styled with CSS for a clean, modern look that adapts to different screen sizes.

Setup

Clone or Download: Download the project files, including index.html.
Dependencies: The project uses Chart.js, loaded via CDN. No additional installations are required.
Run: Open index.html in a web browser. No local server is needed as the project uses a CDN for Chart.js.

Usage

Default Data: The project includes sample orbital distance data (in AU) for a hypothetical planet, with two intentional anomalies (1.20 AU and 0.85 AU).
Custom Data: To use real-world data, modify the orbitData array in the <script> section of index.html with your dataset (e.g., semi-major axis values or distances).
Adjust Anomaly Threshold: Change the threshold value in the JavaScript code (default is 2 * stdDev) to adjust sensitivity for anomaly detection.
View Anomalies: Anomalies are highlighted in red on the scatter plot and listed below the chart with their time step and deviation from the mean.

File Structure

index.html: Main file containing HTML, CSS, and JavaScript for the visualization and anomaly detection.

Example
The sample data visualizes 20 time steps of orbital distances. Two anomalies are detected:

Time T11: 1.20 AU (deviates significantly from the mean).
Time T20: 0.85 AU (deviates significantly from the mean).

Customization

Chart Options: Modify Chart.js options in the <script> section to change chart appearance (e.g., colors, scales, or point sizes).
Anomaly Logic: Replace the standard deviation-based detection with other methods (e.g., z-score, IQR) by updating the anomaly calculation logic.
Styling: Adjust the CSS in the <style> section to customize the layout or appearance.

Notes

The project assumes the data represents orbital distances in astronomical units (AU). Adjust the axis labels and units in the chart configuration if using different metrics.
For large datasets, consider optimizing the chart's performance by limiting the number of displayed points or using Chart.js's data decimation features.

License
This project is unlicensed and free to use or modify for any purpose.
