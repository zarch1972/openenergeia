# openenergeia
Discuss possible collaborative energy tariff / forecasting / battery project

Early spring 2020 has seen many a project spring up around the Octopus Energy API and battery charging.

Folk have been created solutions for the Lux Inverter and the Tesla Powerwall.
https://github.com/celsworth/octolux

This had me thinking that it's great that people are creating one off solutions, but there is lots of common ground in this work, especially around the Octopus API and their Agile tariff.

https://developer.octopus.energy/docs/api/

But wouldn't it be great if there could be a collaborative and open project that worked with a variety of energy tariffs APIs (when more come along) and also battery manfucatuers APIs.

In addition, logic code in the middle that made decisions based on incoming information.

This is how I see a simple flow breakdown.

Inputs
Octopus Energy Agile tariff API
Solcast (solar PV generation forecasts)
Wind forecasting (usually a direct correlation between wind / renewables and cheaper prices on Agile)
Dark Sky?

Logic Box
Take the inputs along with the battery SOC, make decisions about when to overnight(or daytime) charge

Outputs
Battery APIs (Lux / Powerwall / more to come).  There are only a few states; SOC (% full), charge, discharge, be idle.

And finally, a very simple web-based front end.

The number one mandate I see for this is that it has low entry requirements, ie it runs on something as simple and cheap as a Raspberry Pi Zero W

Maybe github isn't the best place to discuss this, maybe there are better places / forums that to happen.  Ideas please?
