# Network Intrusion Detector

A Python tool that monitors network traffic and flags suspicious activity, such as port scans, DDoS-style floods and brute-force attempts, using a machine learning model.

**🚧 In progress. Target: December 2026.**

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white)
![Scapy](https://img.shields.io/badge/Scapy-1F6FEB)
![Status](https://img.shields.io/badge/status-in_progress-orange)

## How it will work
1. **Train:** build features from a public, labelled intrusion dataset (CICIDS2017) and train a classifier that tells normal traffic from attacks.
2. **Capture:** use Scapy to capture live packets and group them into network flows.
3. **Detect:** run each flow through the model and raise an alert when traffic looks malicious.
4. **Show:** display alerts and traffic stats on a simple dashboard.

## Roadmap
- [ ] Set up the project and environment
- [ ] Download and explore the CICIDS2017 dataset
- [ ] Clean the data and select features
- [ ] Train baseline models (Random Forest, Logistic Regression)
- [ ] Evaluate with precision, recall and a confusion matrix
- [ ] Capture live packets with Scapy and build flow features
- [ ] Run the trained model on live traffic and log alerts
- [ ] Test against my own port scans in a lab setup
- [ ] Build a simple dashboard for alerts
- [ ] Write up results

## Tech
- **Python**
- **Scapy** for packet capture
- **scikit-learn** for the machine learning model
- **pandas** and **NumPy** for data processing
- **Wireshark** for checking captures

## Results
Model accuracy, a confusion matrix and screenshots will go here once the first version is done.

## Ethics
This tool only captures traffic on networks and machines I own or have permission to test. All attack testing happens in my own lab.

---
*Personal project by [Akshay Valerio Vanalli](https://github.com/valevana).*
