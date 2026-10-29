# PhotoCandy Queue Simulation and Optimization

## Overview

This project analyzes and optimizes the customer service queue system at PhotoCandy Studio, Tunjungan Plaza 2, Surabaya, Indonesia. The study applies discrete-event simulation to evaluate service performance, identify potential bottlenecks, and determine an improved service configuration.

The analysis covers the complete customer journey, from reservation and photo sessions to photo selection and payment. Simulation models are developed using ExtendSim and optimized using Response Surface Methodology (RSM).

This project was conducted as part of the **Simulation Techniques** course in the Statistics Department, Faculty of Science and Data Analytics, Institut Teknologi Sepuluh Nopember (ITS), in 2025.

## Objectives

- Develop a simulation model representing the existing PhotoCandy service system.
- Evaluate queue performance and server utilization at each service stage.
- Validate the simulation model against observed customer service data.
- Identify service bottlenecks and evaluate alternative server configurations.
- Determine an optimized service configuration to reduce customers' average time in the system.

## Service System

The system consists of four main service stages:

1. **Reservation** — Customers register or make reservations before using the studio.
2. **Photo Session** — Customers use one of three available studio types:
   - Thematic Studio
   - Fisheye Studio
   - Elevator Studio
3. **Photo Selection** — Customers select their photos using one of four available service stations.
4. **Payment** — Customers complete their transactions at the cashier.

## Methodology

The study follows these analytical stages:

1. **Data Collection** — Collect customer arrival times, service start times, and service completion times through direct observation.
2. **Descriptive Analysis** — Examine the characteristics and variability of arrival and service times.
3. **Mean Comparison Tests** — Compare service times across the four photo-selection servers.
4. **Distribution Fitting** — Identify suitable probability distributions for arrival intervals and service times using the Kolmogorov–Smirnov test.
5. **Input Validation** — Compare observed data with simulated input data using the two-sample Kolmogorov–Smirnov test.
6. **System Validation** — Evaluate whether the simulation adequately represents the observed service system.
7. **Discrete-Event Simulation** — Build the initial queue simulation model in ExtendSim.
8. **Optimization** — Apply Response Surface Methodology (RSM) and Central Composite Design (CCD) to evaluate alternative server configurations.
9. **Performance Evaluation** — Compare the initial and optimized models using average time in the system and server utilization.

## Data Collection

Primary data were collected through direct observation at PhotoCandy Studio, Tunjungan Plaza 2, Surabaya.

- **Observation dates:** November 1–2, November 8–9, and November 15–16, 2025.
- **Observation hours:** 14:00–20:00 WIB.
- **Sample size:** 105 customers observed during the study.
- **Data collected:** Interarrival times, reservation service times, studio service times, photo-selection service times, and cashier service times.

## Tools and Technologies

- **ExtendSim 6.0** — Discrete-event simulation and scenario evaluation.
- **Minitab** — Statistical analysis and Response Surface Methodology.
- **SPSS** — Statistical testing and validation.
- **EasyFit** — Probability distribution fitting.
- **Google Sheets** — Data preparation and preliminary calculations.

## Key Findings

The initial simulation identified reservation as a potential bottleneck, with server utilization of 73.6%. The third studio, Elevator Studio, also showed relatively high utilization at 65.5%.

The optimization analysis focused on the reservation stage and Elevator Studio. The recommended configuration adds one server at the reservation stage while retaining one server at Elevator Studio.

| Performance Indicator | Initial Model | Optimized Model |
|---|---:|---:|
| Average time in the system | 1,294.51 seconds | 1,204.16 seconds |
| Average time in the system (minutes) | 21.58 minutes | 20.07 minutes |
| Reservation server configuration | 1 server | 2 servers |
| Elevator Studio server configuration | 1 server | 1 server |

The optimized simulation reduced the average time in the system by approximately **90.35 seconds (7.0%)**. A Mann–Whitney test also indicated a statistically significant difference between the initial and optimized simulation outputs (*p* = 0.003).

These results suggest that increasing reservation capacity can improve overall service efficiency. The recommended configuration is a simulation-based result and should be evaluated against actual operational costs and staffing constraints before implementation.


## Team Members

| Name | Student ID |
|---|---|
| Danella Citra Aldarena | 5003231003 |
| Maria Immaculata Dyah Hita Widowati | 5003231027 |
| Andyka Nabil Putra | 5003231140 |
| Faiz Nabilianto | 5003231143 |

## Academic Information

- **Course:** Simulation Techniques
- **Department:** Statistics
- **Faculty:** Faculty of Science and Data Analytics
- **Institution:** Institut Teknologi Sepuluh Nopember (ITS)
- **Location:** Surabaya, Indonesia
- **Year:** 2025

## Conclusion

This project demonstrates how discrete-event simulation and Response Surface Methodology can be applied to analyze and improve a real-world service queue. Based on the simulation results, adding one reservation server is recommended to reduce the average customer time in the system and improve the balance of server utilization.
