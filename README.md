# openenergeia
Discuss possible collaborative energy tariff / forecasting / battery project

Early spring 2020 has seen many a project spring up around the Octopus Energy API and battery charging.

See discussions in tweets from https://twitter.com/energystatsuk and inspired by my website: https://www.energy-stats.uk/

Folk have been created solutions for the Lux Inverter and the Tesla Powerwall.
https://github.com/celsworth/octolux

This had me thinking that it's great that people are creating one off solutions, but there is lots of common ground in this work, especially around the Octopus API and their Agile tariff.

https://developer.octopus.energy/docs/api/

But wouldn't it be great if there could be a collaborative and open project that worked with a variety of energy tariffs APIs (when more come along) and also battery manfucatuers APIs.

In addition, logic code in the middle that made decisions based on incoming information.

This is how I see a simple flow breakdown.

## Inputs
- Octopus Energy Agile tariff API
- Solcast (solar PV generation forecasts)
- Wind forecasting (usually a direct correlation between wind / renewables and cheaper prices on Agile)
- UK Carbon intensity
- Dark Sky (for weather / cloud forecasting)
- Local configuration parameters (number of batteries, size of batteries, target % full, daily electrical kWh usage etc)


## Logic Box / The Brains
- Take the inputs (from above) along with the battery SOC(%), make decisions about when to overnight(or daytime) charge


## Outputs
- Battery APIs (Lux / Powerwall / more to come).  There are only a few states; SOC (% full), charge, discharge, be idle.

## Front-end
- A very simple web-based front end.

## Hardware Requirements

The number one mandate I see for this is that it has low entry requirements, ie it runs on something as simple and cheap as a Raspberry Pi Zero W

## Points for discussion

- Maybe github isn't the best place to discuss this, maybe there are better places / forums that to happen.  Ideas please?
- Are there projects already out there doing something similar, please link.
- Are there more inputs worth considering?
- Anything around this idea of logic around time of use tariffs and weather forecasting would be fantastic.

Please add anything as a comment in the issue: Discussions points and comments here
https://github.com/zarch1972/openenergeia/issues
