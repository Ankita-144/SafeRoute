# SafeRoute

SafeRoute is a risk-aware navigation system that integrates real-world accident data into route planning. Instead of optimizing only for speed, it enables users to choose safer routes based on historical crash severity.

## Problem Statement

Current navigation systems optimize for shortest or fastest paths but ignore accident risk. This leads users through high-risk zones without any awareness of potential danger.

## Solution

SafeRoute introduces a risk-based routing approach by combining:

* Historical accident data from Bengaluru Traffic Police
* MoRTH Weighted Severity Index (WSI)
* Real-time route computation

The system provides both the safest route and the shortest route, allowing informed decision-making.

## Key Features

* Live risk map with color-coded danger zones
* Dual-route system (safest vs shortest)
* Route risk score based on accident severity
* 2-year trend comparison of accident-prone areas (2023-2024) from open city 

## Risk Model

The system uses the official MoRTH formula:

WSI = (41 × Fatal Accidents) + (1 × Non-Fatal Accidents)

This prioritizes fatal incidents significantly higher, aligning with national road safety standards.

## Tech Stack

* Mapping: Leaflet.js, OpenStreetMap
* Routing: OSRM
* Geocoding: Nominatim
* Data Source: Bengaluru Traffic Police (OpenCity dataset)

## Live Demo

https://xkcq2y.csb.app/

## Source Code

https://codesandbox.io/p/sandbox/traffic-forked-xkcq2y

## Impact

* Introduces safety-aware navigation
* Makes government data accessible to citizens
* Helps reduce exposure to accident-prone routes

## Project Status

This is a functional MVP built entirely client-side with zero paid APIs. But paid api will help in getting correct duration of travelling from one place to other.

## Future 
Crowd based reporting will be helpful as it will be updated real time and with any city data this project is highly deployable

## Authors

Ankita Kumari
Anuttoma Sil
