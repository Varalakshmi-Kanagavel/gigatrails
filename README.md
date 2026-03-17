# GigaTrails AI

AI-powered parametric income protection for gig delivery workers.

## Phase Status

This repository is currently focused on **Phase 1: Research and Planning**.

## Problem

Delivery partners in platforms like Swiggy, Zomato, Blinkit, and Zepto depend on daily operations for weekly income. Environmental and social disruptions can reduce working hours and create income instability.

Key disruption types:

- Heavy rainfall and flooding
- Heatwaves
- Severe air pollution
- Curfews and zone restrictions

## Solution Summary

GigaTrails AI uses a **parametric insurance model**. Instead of manual claims, payouts are triggered automatically when predefined disruption conditions are met and verified.

The system is designed to protect **income continuity** only. It does not cover accident, health, or vehicle repair insurance.

## Core System Layers

### 1. Risk Intelligence

- Estimates disruption probability per city/zone
- Uses historical weather and disruption patterns
- Supports dynamic premium recommendations

### 2. Disruption Monitoring

- Tracks weather, AQI, and local disruption feeds
- Detects threshold-based trigger events in real time

### 3. Smart Verification

- Validates worker presence in affected zone (GPS)
- Checks delivery activity drop signals
- Confirms event with weather/AQI APIs
- Optional: image-based local condition confirmation

### 4. Automated Compensation

- Estimates income loss from disruption duration and average earnings
- Adds compensation into weekly payout flow

## Sample Trigger Framework

Environmental triggers:

- Rainfall above threshold
- Heat index above threshold
- Flood alert in active zone
- AQI in severe range

Social triggers:

- Local curfew
- Zone shutdown
- Restricted movement area

## Weekly Premium Model (Illustrative)

Premium depends on city risk, disruption history, pollution, and rider operating profile.

| City      | Risk Level | Weekly Premium |
| --------- | ---------- | -------------- |
| Bangalore | Low        | INR 25         |
| Mumbai    | Medium     | INR 35         |
| Delhi     | High       | INR 45         |

## Target User Persona

Primary users are food and grocery delivery riders who:

- Depend on daily completed orders for earnings
- Work primarily outdoors
- Need low-friction mobile workflows
- Are highly sensitive to environmental disruptions

## Phase 1 Scope

Phase 1 deliverables in this repository:

- Problem framing and domain analysis
- User persona and scenario definition
- Parametric trigger and verification strategy
- High-level architecture and workflow design
- Documentation and planning artifacts

Out of scope for Phase 1:

- Production deployment
- Real money payout integration
- Full-scale mobile app release

## Planned Roadmap

### Phase 2 (MVP)

- Rider registration and policy setup
- Dynamic premium computation service
- Trigger detection pipeline
- Automated claim and payout simulation

### Phase 3 (Advanced)

- Fraud and anomaly detection enhancements
- Predictive disruption alerts
- Ops and impact analytics dashboard

## Proposed Tech Stack

- **Frontend:** Flutter (mobile-first)
- **Backend:** FastAPI (REST services)
- **Data/ML:** Python, scikit-learn, pandas, numpy
- **Database:** PostgreSQL or Supabase
- **External APIs:** OpenWeather, AQI providers, Maps/Geolocation
- **Payout Simulation:** Razorpay Sandbox or Stripe Test Mode

## Repository Notes

- Architecture diagram and workflow assets can be added under a future `docs/` directory.
- This README will evolve as Phase 1 outputs are finalized.

---

# Innovation Highlights

GigaTrails AI introduces an automated parametric insurance system specifically designed for gig delivery workers.

Key innovations include:

- AI-driven risk-based premium calculation
- automated claim settlement without manual intervention
- real-time environmental disruption monitoring
- multi-factor verification using GPS, environmental APIs, and optional camera input
- mobile-first design tailored for gig workers

By combining artificial intelligence, environmental data, and automated insurance logic, GigaTrails AI provides gig workers with a reliable and scalable financial safety net.

---

If you want, I can also give you:

• **the best system architecture diagram to include in the README**
• **a better AI model design section (to impress judges)**
• **a database schema for this project**
• **a 2-minute demo video script**

These will make your submission **look like a top 5 project in DevTrails.**
