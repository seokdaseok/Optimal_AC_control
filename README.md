# Optimal_AC_control

## Introduction

Air conditioning (AC) accounts for a large proportion of total electricity usage in buildings, which necessitates an efficient AC automatic control strategy. This study proposes an optimization-based dynamic AC control system that aims to not only retain human comfort level but also save energy consumption. Specifically, we introduce a machine learning-based temperature prediction model to forecast the outside temperature in future horizons. Based on the predicted outside temperature, we formulate linear programming to optimize the AC's strategies for a future period that integrates the physical thermal model to capture temperature changes over time. The objective function is a weighted summation of human discomfort levels and energy consumption. The decision variables are how much heat the AC should take out (cooling) or bring in (heating) during each time interval for each room. The final control strategies are implemented in a rolling horizon manner, where at the start of each time interval, we solve the model for the future but only implement the actions of the current time step. The model is validated using two classrooms in Independent Schools Foundations (ISF), an international school in Hong Kong as the case study. Results show that the proposed methods can well control the temperature around the target. It outperforms typical on-off control methods with 57.7% less energy consumption and 44.2% less human discomfort levels in summer, and 62.1% less energy consumption and 5.01% less human discomfort levels in the winter. 

## Data

The temperature data comes from an open-source data set by the Hong Kong Observatory. The classroom data, number of people in the classroom data, and AC configuration data were provided by the ISF Academy.

## Referrence

## Competition

The model and code are used for the ISEF 2023 Competition.
