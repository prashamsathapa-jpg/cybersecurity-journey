# Suricata IDS Lab Notes

## Overview
This project contains my learning notes and practical exercises from the Google Cybersecurity Certificate.

## Tool Used
- Suricata IDS/IPS
- Linux Terminal
- jq

## Skills Practiced
- Writing Suricata rules
- Analyzing network traffic
- Reading IDS alerts
- Investigating logs

## Suricata Rule Structure

A Suricata rule contains:

1. Action
2. Header
3. Rule options

Example concepts learned:
- alert
- flow
- content
- sid
- rev

## Commands Practiced

```bash
cat custom.rules

sudo suricata -r sample.pcap -S custom.rules -k none

cat /var/log/suricata/fast.log

jq . /var/log/suricata/eve.json | less