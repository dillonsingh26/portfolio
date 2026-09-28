+++
title = 'StatusTix'
description = 'Founder & Sole Developer · 2026–Present'
summary = 'Founder & Sole Developer · 2026–Present. A social sports app where fans earn status for showing up, built on a verified cross-league attendance graph spanning 27 leagues.'
weight = 20
tags = ['TypeScript', 'Firebase', 'Mixpanel', 'Product analytics']
+++

StatusTix is a social sports app designed for fans to earn status. It started as a Streamlit prototype in a Northwestern sports analytics course. After the course I founded the company and rebuilt the product as a production iOS app.

For the technical details, see the [StatusTix project page]({{< relref "/projects/statustix" >}}).

## Building the product

- Designed and built a full-stack consumer iOS app around a verified cross-league fan-attendance graph, with a two-ledger data model that separates GPS-verified check-ins from self-reported ones.
- Curated a geospatial dataset covering 27 leagues, more than 2,600 teams, and more than 2,500 venues.
- Built a photo-based game-detection pipeline that matches camera-roll GPS and timestamps against venue coordinates and league schedules.
- Maintained 489 automated Jest tests across 31 suites, with Firebase, Sentry monitoring, and EAS CI/CD.

## Running the business

- Designed the monetization strategy: a loyalty and promotions network for teams, leagues, and merchandisers built on aggregated attendance data. This included the business plan, Lean Canvas, and revenue forecasts.
- Defined and instrumented the full product-metrics stack in Mixpanel, with a standardized event taxonomy across acquisition, onboarding, activation, engagement loops, and growth mechanics.
- Ran competitive analysis of incumbent apps and adjacent threats, identifying verified provenance and the social feed as the differentiators.
- Replaced a points system with gated status tiers that reward breadth — leagues, venues, and playoff games — over volume, so that user incentives line up with data coverage.
