+++
title = 'StatusTix'
description = 'A social sports app where fans earn status for showing up.'
summary = 'A social sports iOS app built on a verified cross-league fan-attendance graph — 27 leagues, 2,600+ teams, and 2,500+ venues. Founder and sole developer.'
weight = 10
tags = ['TypeScript', 'Firebase', 'Mixpanel', 'Product analytics', 'Sports']
+++

StatusTix is a social sports app designed for fans to earn status. Fans check in at the games they attend, and the app builds a verified record of their attendance across leagues.

I'm the founder and sole developer. The first version was a Streamlit prototype built in a Northwestern sports analytics course. I then rebuilt it as a production iOS app.

## By the numbers

| | |
|---|---|
| **Leagues** | 27 |
| **Teams** | 2,600+ |
| **Venues** | 2,500+ |
| **Automated tests** | 489 Jest tests across 31 suites |

## How it works

### A two-ledger attendance model

Attendance is recorded in two separate ledgers: check-ins verified by GPS, and check-ins that are self-reported. Keeping them apart preserves the integrity of the verified data while still letting fans log the games they went to before they had the app.

### Photo-based game detection

The app reads GPS coordinates and timestamps from photos in the camera roll and matches them against venue coordinates and league schedules. Radius-tuned proximity matching, cross-source deduplication, and caching bring a full-library scan down to about 10–15 seconds.

### Schedule and team data

Schedules come from the ESPN and BallDontLie APIs. Fuzzy team-name matching reconciles the differences between sources.

### Status, challenges, and leaderboards

Rule-based engines compute tiered status, challenges, and leaderboards from each fan's attendance history. Status tiers are gated on breadth — leagues, venues, and playoff games — and not on volume alone.

### Product analytics

The full product funnel is instrumented in Mixpanel, with a standard event taxonomy covering onboarding, check-ins, and growth loops.

## Stack

TypeScript, Firebase (Firestore, Auth, Cloud Functions), Mixpanel, Jest, Sentry, EAS CI/CD

## Status

The App Store launch is planned for before December 2026. The source repository is private.
