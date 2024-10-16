---
sccp: 358
title: Deploy More Markets on Perps V3 Base and Arbitrum
network: Base & Arbitrum
status: Draft
type: Governance
created: 2024-10-11
author: Robin (@robin2192), Kaleb
---

# Simple Summary

This SCCP proposes to deploy the below markets on Perps V3 on Base and Arbitrum.

## Base Markets:

| **Market** | **minimumInitialMarginRatio** | **InitialMarginRatio** | **maintenanceMarginScalar** |   **skewScale**   | **maxMarketSize** | **maxMarketValue** |
|:----------:|:-----------------------------:|:----------------------:|:---------------------------:|:-----------------:|:-----------------:|:------------------:|
|    MKR     |                               |                        |                             |                   |                   |                    |
|    POL     |                               |                        |                             |                   |                   |                    |
|    MEW     |                               |                        |                             |                   |                   |                    |
|    POPCAT  |                               |                        |                             |                   |                   |                    |
|    EIGEN   |                               |                        |                             |                   |                   |                    |
|    WLD     |                               |                        |                             |                   |                   |                    |
|    PEOPLE  |                               |                        |                             |                   |                   |                    |
|    ZRO     |                               |                        |                             |                   |                   |                    |
|    RENDER  |                               |                        |                             |                   |                   |                    |
|    NOT     |                               |                        |                             |                   |                   |                    |
|    SATS    |                               |                        |                             |                   |                   |                    |
|    IO      |                               |                        |                             |                   |                   |                    |


## Arbitrum Markets:

| **Market** | **minimumInitialMarginRatio** | **InitialMarginRatio** | **maintenanceMarginScalar** |   **skewScale**   | **maxMarketSize** | **maxMarketValue** |
|:----------:|:-----------------------------:|:----------------------:|:---------------------------:|:-----------------:|:-----------------:|:------------------:|
|    ALGO    |                               |                        |                             |                   |                   |                    |
|    APT     |                               |                        |                             |                   |                   |                    |
|    ARKM    |                               |                        |                             |                   |                   |                    |
|    ATOM    |                               |                        |                             |                   |                   |                    |
|    AXL     |                               |                        |                             |                   |                   |                    |
|    AXS     |                               |                        |                             |                   |                   |                    |
|    BAL     |                               |                        |                             |                   |                   |                    |
|    BCH     |                               |                        |                             |                   |                   |                    |
|    BLUR    |                               |                        |                             |                   |                   |                    |
|    BOME    |                               |                        |                             |                   |                   |                    |
|    BONK    |                               |                        |                             |                   |                   |                    |
|    COMP    |                               |                        |                             |                   |                   |                    |
|    DOT     |                               |                        |                             |                   |                   |                    |
|    ENA     |                               |                        |                             |                   |                   |                    |
|    EOS     |                               |                        |                             |                   |                   |                    |
|    ETC     |                               |                        |                             |                   |                   |                    |
|    ETHBTC  |                               |                        |                             |                   |                   |                    |
|    ETHFI   |                               |                        |                             |                   |                   |                    |
|    FIL     |                               |                        |                             |                   |                   |                    |
|    FLOW    |                               |                        |                             |                   |                   |                    |
|    FTM     |                               |                        |                             |                   |                   |                    |
|    FXS     |                               |                        |                             |                   |                   |                    |
|    GALA    |                               |                        |                             |                   |                   |                    |
|    GRT     |                               |                        |                             |                   |                   |                    |
|    ICP     |                               |                        |                             |                   |                   |                    |
|    IMX     |                               |                        |                             |                   |                   |                    |
|    INJ     |                               |                        |                             |                   |                   |                    |
|    JTO     |                               |                        |                             |                   |                   |                    |
|    JUP     |                               |                        |                             |                   |                   |                    |
|    LDO     |                               |                        |                             |                   |                   |                    |
|    MEME    |                               |                        |                             |                   |                   |                    |
|    PENDLE  |                               |                        |                             |                   |                   |                    |
|    SEI     |                               |                        |                             |                   |                   |                    |
|    SNX     |                               |                        |                             |                   |                   |                    |
|    STRK    |                               |                        |                             |                   |                   |                    |
|    SUI     |                               |                        |                             |                   |                   |                    |
|    SUSHI   |                               |                        |                             |                   |                   |                    |
|    TAO     |                               |                        |                             |                   |                   |                    |
|    TON     |                               |                        |                             |                   |                   |                    |
|    TRX     |                               |                        |                             |                   |                   |                    |
|    W       |                               |                        |                             |                   |                   |                    |
|    YFI     |                               |                        |                             |                   |                   |                    |
|    MEW     |                               |                        |                             |                   |                   |                    |
|    POPCAT  |                               |                        |                             |                   |                   |                    |
|    EIGEN   |                               |                        |                             |                   |                   |                    |
|    WLD     |                               |                        |                             |                   |                   |                    |
|    PEOPLE  |                               |                        |                             |                   |                   |                    |
|    ZRO     |                               |                        |                             |                   |                   |                    |
|    RENDER  |                               |                        |                             |                   |                   |                    |
|    NOT     |                               |                        |                             |                   |                   |                    |
|    SATS    |                               |                        |                             |                   |                   |                    |
|    IO      |                               |                        |                             |                   |                   |                    |


Aside from the above parameters , the perps markets will have the following configurations as well:
- TakerFeeRatio: 10 bp
- MakerFeeRatio: 0 bp
- maxFundingVelocity: 36
- flagRewardRatio: 3 bp
- minimumPositionMargin: 50
- lockedOiRatio: 0.5 
- maxLiquidationLimitMultiplier: 1.5
- maxLiquidationPD: 5 bp
- endorsedLiquidator: "0x11233749514Ab8d00C0A5873DF7428b3db70030f"


# Abstract

The parameters configurations description is as follows:
- initialMarginRatio is a scalar applied on the minimumInitialMarginRatio to determine the minimum initial margin required to support a given portfolio of positions
- maintenanceMarginScalar is a scalar applied on the initialMargin in order to obtain the maintenanceMargin. When traders fall below the maintenance margin, they are liquidated.
- skewScale is the scaling factor of the relevant market in the underlying currency for computing price impact and funding rates
- maxMarketSize is the max market value of the relevant market in the underlying currency
- maxMarketValue is the max market value of the relevant market in USD
- maker/taker fees pertain to fees charged when trading
- maxFundingVelocity is the main parameter that allows to nudge funding rates
- minimumPositionMargin is the minimum margin required
- lockedOiRatio is the multiplier that determines the minimum amount of perp collateral required to back a given perp market
- maxLiquidationLimitMultiplier is a parameter that rate limits liquidations. It is applied on the sum of maker and taker fees with a liquidation rate limit being triggered if pd exceeds that value
- maxLiquidationPD is the minimum pd that triggers a reset of the liquidation capacity
- endorsedLiquidator is a liquidator address that can bypass the rate limit
- the collateral liquidation penalty is the penalty paid to the liquidator for executing a liquidation


# Motivation

The main motivation is to bring the deployed markets on Base and Arbitrum to parity, while also launching additional markets with high caps to both, in order to fully showcase the feature set available with the V3 deploy.

# Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
