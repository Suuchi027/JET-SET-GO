# JET-SET-GO
Python project

# Project Goal: Proactive Resource Planning at ORD
This project delivers the solution for the SkyHack 3.0: United Airlines challenge by developing a data-driven framework to quantify flight complexity.

The core goal is to provide Frontline teams at Chicago O’Hare International Airport (ORD) with a predictive, systematic score (0.0 to 1.0) and classification (Easy, Medium, Difficult) for every flight. This enables proactive resource planning and optimized allocation before flights become delayed or over-stressed.

## The Problem Solved
Our system addresses this by identifying high-difficulty flights driven by compounding factors like limited ground time, high passenger load, and specific customer service needs—the exact causes of operational strain.

## Key Methodology & Features
The scoring model is a composite index built from five primary operational complexity features, engineered from the provided flight, PNR, remark, and bag datasets:

Tight Turn Score: Measures scheduled ground time against the minimum_turn_minutes. (The dominant complexity driver).

Load Factor: Passenger volume (total_pax) relative to total_seats.

Total Bags Count: Sum of Origin and Transfer bags (identifying high baggage volume).

SSR/PAX Ratio: Ratio of special service requests (special_service_request) to total passengers (total_pax).

International Indicator: A fixed score boost for non-U.S. arrivals (accounting for customs, long-haul, and documentation complexity).

## Project Structure and Technologies
Programming Language: Python
Key Libraries: pandas, numpy, matplotlib, seaborn.

