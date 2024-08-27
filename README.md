
# Network Traffic Analyzer

This Python application offers a comprehensive, user-friendly interface for capturing and analyzing network packets in real time. The application displays captured packets with color-coded protocol details, generates real-time visualizations of packet counts, and sends email alerts when network traffic exceeds a predefined threshold.

## Features

- **Packet Capture**: Capture packets from a specified network interface and save them to a PCAP file.
- **Detailed Packet Display**: Display captured packet information in a text widget, including protocol, source IP, and destination IP, with color-coding for easy identification (TCP in blue, UDP in green, etc.).
- **Real-Time Visualization**: Generate and display real-time visualizations of packet counts over time using Matplotlib.
- **Email Alerts**: Automatically send email alerts when network traffic exceeds a user-defined threshold, ensuring immediate notification of potential issues.
- **Flexible Capture Management**: Start and stop packet capture on demand, with an option to stop the capture before the specified duration.

## Requirements

- **Python 3.x**
- **tkinter**: GUI library (included in standard Python installation)
- **pyshark**: For packet capturing (`pip install pyshark`)
- **threading**: For managing capture processes (included in standard Python installation)
- **time**: For managing timing and delays (included in standard Python installation)
- **smtplib**: For sending emails (included in standard Python installation)
- **email**: For email content handling (included in standard Python installation)
- **matplotlib**: For generating visualizations (`pip install matplotlib`)

## Installation

Install the required libraries using pip:

```bash
pip install pyshark matplotlib
```

Clone or download the repository containing the Python script (`packet_capture_display.py`).

## Usage

1. Open a terminal or command prompt and navigate to the directory containing the script.
2. Run the script using:

   ```bash
   python packet_capture_display.py
   ```

3. Follow the on-screen instructions to begin capturing packets and analyzing network traffic.

## Configuration

Customize the following values in the script to suit your needs:

- `EMAIL_ADDRESS`: Your email address for sending alerts.
- `EMAIL_PASSWORD`: Your email password for sending alerts.
- `RECIPIENT_ADDRESS`: The email address where alerts should be sent.
- `ALERT_THRESHOLD`: Packet count threshold that triggers email alerts.

## GUI Elements

- **Network Interface**: Displays "Wi-Fi" by default; modify the script to select from available interfaces.
- **PCAP File Path**: Enter the desired path to save captured packets. A browse button is provided for easy selection.
- **Capture Duration**: Specify the capture duration in seconds.
- **Start Capture Button**: Click to start capturing packets.
- **Stop Capture Button**: Click to stop the capture before the specified duration (optional).
- **Text Widget**: Displays captured packet details, color-coded by protocol.
- **Visualization**: A real-time plot showing packet count over time.

## Example Output

- **Packet Details**: The text widget will display captured packet details (protocol, source IP, destination IP) with color-coding for easy analysis.
- **Real-Time Visualization**: A Matplotlib plot will visually represent packet counts over time.
- **Email Alerts**: When the packet count exceeds the predefined threshold, an email alert will be sent to the specified recipient.

## Disclaimer

Please note that sending emails from Python scripts may require additional configuration depending on your email service provider. For Gmail users, enabling "Less secure app access" might be necessary. Consult your email provider's documentation for similar settings if applicable.

## License

This project is licensed under the MIT License. See the LICENSE file for details.


