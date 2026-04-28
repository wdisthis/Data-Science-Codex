---
tags:
  - statistik/lanjutan
aliases:
  - Stasioneritas
date: 2026-04-28
status: complete
---

# Stationarity

> **Ringkasan:** Properti time series di mana mean dan variance konstan sepanjang waktu.

## Mengapa Penting

Banyak model time series (ARIMA, dll.) mengasumsikan data stasioner.

## Uji Stasioneritas

- **ADF Test** (Augmented Dickey-Fuller)
- **KPSS Test**

## Cara Membuat Data Stasioner

- Differencing (d=1, d=2)
- Log transformation

## Hubungan dengan Konsep Lain

- Terkait: [[Autocorrelation]], [[Time Series Forecasting]]
- Library: [[Statsmodels]]