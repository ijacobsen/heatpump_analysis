## Scope


This was a quick project to help me analyze the operating costs between two different model Mitsubishi heat pumps for my home. 

Historical temperature data from Laguardia Airport was collected from the NOAA database using their API.

Mitsubishi provides some benchmark performance stats for their units - the rated input kW and the rated BTU output for 47F and 17F outdoor temperatures. From my own research it's a reasonable assumption to make that the coefficient of performance (COP) within that operating range is nearly linear, so I modeled the COP within that temperature band with a simple regression.

With the COP model and the daily outdoor temperature for the past 20 years I calculated how much my estimated electricity costs would be with constant heat pump operation delivering 24k BTU (manual J performed on my well insulated apartment).

Two Mitsubishi models were compared - the standard model and the hyper heat model. The hyper heat has a better COP throughout the entire temperature band, and is also capable of delivering BTU's in temperatures below what the standard model can deliver. The hyper heat model is more expensive than the standard model so this analysis was to see how significant the cost difference is considering the differences in electricity use during usage.

In conclusion using the hyper heat model saves approximately $200/year in operating costs, and after about 4 years it covers the difference in initial cost.
