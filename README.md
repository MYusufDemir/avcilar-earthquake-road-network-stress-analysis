# Avcılar Earthquake Road Network Stress Analysis

This repository contains an interactive web-based report for a scenario-based road network stress analysis of Avcılar under a major earthquake scenario.

## Project Scope

The study investigates:

- road segments that may be exposed to closure risk under a major earthquake scenario,
- open road segments that may experience increased network stress after disruptions,
- candidate local bottlenecks,
- critical open backbone roads,
- and the difference between the immediate post-earthquake condition (T0) and the partial recovery stage after the first 4–5 hours (T1).

## Methodological Summary

The analysis uses:

- OpenStreetMap-based vehicle road network data,
- neighborhood-level building indicators,
- building age and floor-count based risk proxies,
- road-type vulnerability assumptions,
- normalized road length,
- graph-based betweenness centrality,
- T0 closure scenario logic,
- T1 reopening and remaining-closure logic.

The closure-risk model combines building-related neighborhood risk, road-type vulnerability, and normalized road length. After assumed closures are removed from the network, centrality is recalculated to identify stress corridors and candidate bottlenecks.

## Scenario Definitions

- **T0:** Immediate post-earthquake condition.
- **T1:** First 4–5 hours after the earthquake, representing a partial recovery stage in which some roads may have been reopened depending on road hierarchy, network centrality, and lower building-related risk.

## Map Layers

- **Black:** roads assumed to be closed,
- **Orange:** main stress corridors,
- **Purple:** candidate local bottlenecks,
- **Green:** critical open backbone roads,
- **Gray:** background road network.

## Limitations

This analysis is not a deterministic damage or road closure prediction. It does not include real-time traffic volumes, observed earthquake damage, detailed structural vulnerability of bridges or viaducts, emergency response team locations, or actual operational road-clearing constraints. The outputs should be interpreted as relative risk and stress indicators under the adopted assumptions.

## Prepared by

**Muhammet Yusuf Demir**  
Istanbul Technical University  
Industrial Engineering
