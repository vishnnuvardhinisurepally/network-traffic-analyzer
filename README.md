# Network Traffic Analyzer

Description

This Python application provides a user-friendly interface for capturing network packets, displaying them in a text widget with color-coded protocols, and generating real-time packet count visualizations. Additionally, it features email alerts when network traffic exceeds a predefined threshold.

Features

Capture packets from the specified network interface.
Save captured packets to a PCAP file.
Display captured packet information in a text widget, including protocol, source IP, and destination IP.
Color-code captured packets based on protocol (TCP and UDP).
Generate real-time visualizations of packet count over time using Matplotlib.
Send email alerts when network traffic exceeds a user-defined threshold.
Optionally stop capture before the specified duration using a dedicated button.

Requirements

Python 3.x
tkinter library (included in standard Python installation)
pyshark library (pip install pyshark)
threading library (included in standard Python installation)
time library (included in standard Python installation)
smtplib library (included in standard Python installation)
email library (included in standard Python installation)
matplotlib library (pip install matplotlib)
Installation

Install the required libraries using pip:

Bash
pip install pyshark matplotlib
Use code with caution.

Clone or download the repository containing the Python script (packet_capture_display.py).

Usage

Open a terminal or command prompt and navigate to the directory containing the script.

Run the script using:

Bash
python packet_capture_display.py
Use code with caution.

Configuration

Update the following values in the script to customize your application:
EMAIL_ADDRESS: Your email address (for sending alerts).
EMAIL_PASSWORD: Your email password (for sending alerts).
RECIPIENT_ADDRESS: Email address to receive alerts.
ALERT_THRESHOLD: Packet count threshold for triggering email alerts.
GUI Elements

**Network Interface**: Currently displays "Wi-Fi." You can modify the script to allow selection from available interfaces.
**PCAP File Path**: Enter the desired path to save captured packets. A browse button is provided for convenience.
**Capture Duration**: Specify the duration (in seconds) for the capture.
**Start Capture Button**: Initiates the capture process.
**Stop Capture Button**: Stops the capture before the specified duration. (Optional)
**Text Widget**: Displays captured packet information and is color-coded based on protocol.
**Visualization**: A plot showing packet count over time.

Example Output

The text widget will display captured packet details, and the plot will visually represent the packet count over time. When the threshold is crossed, an email alert will be sent.

Disclaimer

Please note that sending emails from Python scripts might require additional configuration depending on your email service provider. Make sure to enable "Less secure app access" in your Gmail settings or consult your email provider's documentation for similar settings if applicable.


