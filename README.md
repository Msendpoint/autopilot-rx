# AutopilotRx

> Automated pre-flight diagnostics and remediation toolkit for IT admins who need Autopilot deployments to succeed the first time, every time.

## Overview

AutopilotRx is a PowerShell-based diagnostic and remediation toolkit that runs pre-deployment checks on devices before they ship, validates network endpoint reachability, detects stale Autopilot objects, and generates a plain-English failure report with one-click fix scripts. It integrates with Intune via Graph API to surface hash registration issues, ESP configuration drift, and MDM enrollment URL blockers before a remote user ever sees an error screen. A companion lightweight web dashboard lets MSPs track fleet-wide Autopilot health across multiple tenants.

## Problem This Solves

Eliminates the costly, embarrassing failure loop of shipping a laptop to a remote user only to have it brick on the Enrollment Status Page — requiring expensive return shipping, IT overtime, and lost employee productivity — by catching every common root cause before the device leaves the building

## Target Audience

MSP technicians and in-house IT admins managing Autopilot deployments across 200+ devices, especially those supporting remote or distributed workforces where on-site remediation is impossible

## Tech Stack

PowerShell, Microsoft Graph API, Azure Functions, React, Node.js

## Quick Start

```powershell
# Clone the repository
git clone https://github.com/autopilot-rx.git
cd autopilot-rx

# One-click install & run
.\Install.ps1

# Or run the script directly
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
.\scripts\{autopilot-rx}.ps1
```

## Usage

Runs a comprehensive pre-deployment validation sweep that checks Autopilot hash registration status, tests reachability of all required MDM enrollment endpoints, identifies stale or duplicate Autopilot device objects in Intune, and outputs a color-coded remediation report with executable fix commands for each detected issue.

## Monetization Strategy

Tiered pricing sold via Gumroad and GitHub Sponsors: Core PowerShell toolkit at $49 one-time for solo admins; Pro bundle with multi-tenant Graph API integration and web dashboard at $29/month per MSP on Lemon Squeezy; Enterprise license with white-labeling at $299/month. Upsell a 2-hour remote remediation consulting session at $250 flat for teams with active deployment fires.

| Metric | Value |
|--------|-------|
| Revenue Potential | HIGH |
| Estimated Effort  | 1-3months |

## About the Author