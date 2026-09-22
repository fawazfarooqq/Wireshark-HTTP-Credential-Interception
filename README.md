# Wireshark-HTTP-Credential-Interception
Hands-on Wireshark lab demonstrating how plaintext credentials can be exposed when transmitted over unencrypted HTTP.
# Wireshark HTTP Credential Interception Lab

## Overview

A hands-on network security lab demonstrating the risks of transmitting sensitive information over unencrypted HTTP.

The project uses Wireshark to capture network traffic generated while submitting a test web form over HTTP and analyzes the resulting packets to demonstrate how plaintext form data can be exposed.

## Objective

- Capture HTTP network traffic using Wireshark
- Analyze TCP/HTTP packets
- Identify form data transmitted over HTTP
- Demonstrate why plaintext HTTP is insecure
- Understand the importance of HTTPS/TLS encryption

## Tools Used

- Wireshark
- Google Chrome
- HTTP
- TCP/IP
- httpbin.org

## Lab Workflow

1. Started Wireshark and captured traffic from the Wi-Fi interface.
2. Opened a test HTTP form.
3. Entered dummy information into the form.
4. Submitted the form.
5. Captured the resulting network packets in Wireshark.
6. Inspected the HTTP request and server response.
7. Observed the submitted form data in the HTTP response.

## Evidence

### Test Form
![Test Form](screenshots/vulnerable-form.jpg)

### Wireshark Packet Capture
![Wireshark Capture](screenshots/wireshark-capture.jpg)

### Captured HTTP Data
![Captured Data](screenshots/captured-data.jpg)

## Security Impact

HTTP does not provide encryption for application data. An attacker who can observe the network traffic may be able to read sensitive information transmitted through an HTTP connection.

This demonstrates why HTTPS/TLS should be used when transmitting credentials or other sensitive information.

## Disclaimer

This project was performed in a controlled environment using test data for educational and cybersecurity learning purposes.
