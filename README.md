# vps-maintenance-n8n
# **N8n workflows to monitor and maintain my Hostinger VPS**

## **This N8n workflow checks for available package updates on an Ubuntu VPS and sends a Telegram alert if updates are found. It helps automate basic system maintenance.**

Steps:

Cron node triggers the workflow at regular intervals.

SSH node runs apt list --upgradable on the VPS.

Set node formats the output to count upgradable packages.

IF node checks if the count is greater than zero.

Telegram node sends a message with the number of packages to update.
