# Pd_share
python function to measure the information share and component share
IS and CS only accurately measure contribution to price discovery, in
the conventional sense of being the first to reflect innovations in the fundamental value,
when the price series being compared have a similar level of noise. 

the function does the following :
- Estimate Vector Error Correction Model (VECM): Using the return series, estimate the VECM to capture the relationships between the price series from different trading venues. This involves determining the cointegration relationships between the price series and the error correction term, which measures how the price series adjust to deviations from the long-run equilibrium relationship.
- Calculate the speed of adjustment coefficients: Obtain the speed of adjustment coefficients from the VECM estimation. These coefficients indicate how quickly each trading venue reacts to new information and returns to the equilibrium relationship.
- Compute the Information Share: Using the speed of adjustment coefficients, compute the Hasbrouck Information Share for each trading venue. This measure represents the proportion of total price discovery attributable to each venue.
- Calculate the absolute price changes: Compute the absolute price change for each trade in each trading venue.
- Sum the absolute price changes: Calculate the sum of the absolute price changes for each trading venue.
- Compute the Component Share: Calculate the proportion of the total sum of absolute price changes attributable to each trading venue. This proportion represents the HMW Component Share for each venue, reflecting its contribution to the overall price discovery process.
