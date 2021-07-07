# Billing Logic

## Comms credits top up / remaining tracking

Anything that is not inclusive minutes is charged through comms credits.

There is no API to get current comms credit total, so customer must input the current total periodically and their current top up. This is how we calculate credit remaining

Due to timing inconsistency modality calculation of remaining comms credits will not be 100% accurate, it could be out by around a days typical usage. The idea is not to be 100% accurate on remaining credit but to know exactly how much was used in a particular period

The goal is to alert when there is less than X in the comms credits pot. We recommend this alert is set higher than 5 days typical usage.

## Comms credits usage tracking

Many things can use comms credits, Billing will report on anything that uses comms credits. Anything with a per minute cost is from comms credits.

We report on all of them to show correct burn down

## Conferencing comms credits cost

- PSTN dial in toll free (conf_in and TollFree and capability MCOPSTNPP)
- conf_in or conf_out and PPM (conf_in and capability MCOMEETACPEA) 






