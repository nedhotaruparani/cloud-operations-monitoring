# Google Cloud Operations Monitoring

## Project Overview

This project demonstrates website uptime monitoring, alert configuration, email notifications, and centralized log exploration using Google Cloud Operations.

The goal is to monitor website availability, detect potential failures, and notify the monitoring team through email alerts.

## Technologies Used

- Google Cloud Platform (GCP)
- Cloud Monitoring
- Cloud Logging
- Uptime Checks
- Alerting Policies
- Email Notification Channels
- Logs Explorer

## Architecture and Implementation

### 1. Website Uptime Monitoring

Configured an HTTPS uptime check for `example.com`.

Configuration:
- Protocol: HTTPS
- Port: 443
- Request path: `/`
- Check interval: 5 minutes
- Timeout: 10 seconds
- SSL certificate validation: Enabled
- Monitoring locations: Global

### 2. Alert Configuration

Created an uptime alert policy to detect website availability issues.

Configuration:
- Metric: Uptime Check URL – Check passed
- Threshold: Below 99%
- Retest window: 1 minute
- Notification channel: Email

### 3. Email Notifications

Configured an email notification channel to receive alerts when the uptime condition is violated.

Successfully tested alert generation and email delivery using a temporary test policy. The temporary policy was deleted after successful validation.

### 4. Monitoring Dashboard

Created a Cloud Monitoring dashboard with an uptime scorecard.

Observed uptime result: **100%**

### 5. Log Exploration

Used Cloud Logging Logs Explorer to explore logs and audit events in the GCP project.

## Validation and Testing

The project was validated through the following checks:

- Verified HTTPS uptime check configuration.
- Confirmed successful website availability monitoring.
- Verified the uptime metric.
- Tested alert generation using a temporary threshold.
- Confirmed email notification delivery.
- Removed the temporary test alert policy after validation.

## Project Outcome

Successfully implemented a basic cloud operations monitoring solution using Google Cloud Monitoring and Logging.

The project demonstrates practical experience with uptime monitoring, metric-based alerting, email notifications, dashboard configuration, and log exploration.

## Screenshots

Screenshots will be added in the `screenshots` folder:

1. Uptime Check Configuration
2. Monitoring Dashboard
3. Alert Policy Configuration
4. Email Alert Notification
5. Logs Explorer
6. Email Notification Channel

## GCP Project

`cloud-ops-monitoring-2026`

**Note:** The uptime check uses `example.com` as a demonstration endpoint. This project is a learning and portfolio project.
