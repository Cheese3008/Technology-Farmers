# Technology Farmers

Technology Farmers is an IoT-based water quality monitoring system for aquaculture, combining embedded sensing, realtime data visualization, backend integration, and an assistant-style analysis module for water quality assessment and recommendations.

## Overview

This project is designed to monitor important water-quality indicators in aquaculture environments and present them through a user-friendly dashboard. The system integrates sensor acquisition, realtime visualization, and an analysis workflow that transforms current sensor readings into concise risk assessments and practical recommendations for operators.

The project focuses on building a complete applied system that connects IoT monitoring with intelligent user-facing analysis.

## Objectives

- Monitor key water-quality parameters in realtime
- Visualize sensor data clearly through a dashboard
- Support quick interpretation of water conditions
- Extend traditional IoT monitoring with an assistant-based analysis workflow
- Explore practical Prompt Engineering for sensor-to-insight interaction

## Main Components

### 1. firmware_esp32s3
Embedded firmware for ESP32-S3 responsible for:
- reading sensor values
- preparing sensor payloads
- publishing data for downstream monitoring modules

### 2. Spring Boot
Backend module responsible for:
- system-side integration
- API and service expansion
- supporting future data processing and storage workflows

### 3. web
Realtime dashboard responsible for:
- displaying water-quality indicators such as turbidity, temperature, and pH
- rendering live charts
- providing a clean operator interface
- integrating an assistant-style interaction layer for water-quality interpretation

### 4. prompt_engineering
Prompt Engineering module responsible for:
- defining prompt templates for water-quality assessment
- structuring sensor-to-language analysis flows
- generating concise, understandable guidance from current sensor readings
- supporting recommendation-oriented interaction for aquaculture monitoring

## Current Features

- Realtime monitoring dashboard
- Visualization of turbidity, temperature, and pH
- Live charts for sensor trends
- Dark mode UI
- Assistant-style water-quality analysis
- Prompt-based risk assessment and recommendation workflow
- Modular project structure for firmware, backend, web, and analysis components

## Prompt Engineering Integration

A dedicated Prompt Engineering branch is integrated into the project to support natural-language analysis of current water conditions.

This module is designed to:
- interpret current sensor readings
- assess the overall water-quality condition
- identify potential risks
- provide short, practical recommendations for operators

The goal is to move beyond raw sensor display and toward an interaction model where system data can be translated into actionable operational insight.

## Water Quality Analysis Workflow

The analysis flow is organized as follows:

1. Collect current sensor readings from the monitoring pipeline
2. Structure those readings into an analysis-ready input format
3. Apply a prompt template for water-quality interpretation
4. Produce a short assessment including:
   - risk level
   - explanation
   - recommended action

This workflow provides a foundation for future integration with more advanced AI services.

## Folder Structure

```text
TF/
├── firmware_esp32s3/
├── Spring Boot/
├── web/
│   └── src/
│       └── index.html
├── prompt_engineering/
│   ├── README.md
│   ├── prompt_templates.md
│   └── sample_cases.json
├── .env.example
├── .gitignore
└── README.md
```

## System Scope

The project currently covers:
- IoT data acquisition layer
- dashboard visualization layer
- backend integration layer
- assistant-based analysis layer

This makes the repository suitable as both an applied IoT project and an extended AI-assisted monitoring system.

## Future Development

- integrate long-term historical data storage
- improve alerting and threshold logic
- connect backend-side AI services for production-ready analysis
- support richer decision-support workflows for aquaculture operation
- expand the assistant into a more complete water-management support tool

## Tech Stack

- ESP32-S3
- MQTT
- Spring Boot
- HTML / CSS / JavaScript
- Chart.js
- Prompt Engineering workflow design

## Project Direction

Technology Farmers is positioned as an applied IoT + intelligent monitoring project, where embedded sensing and realtime dashboards are combined with language-based analysis to create a more practical operator experience.
