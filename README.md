# WHOIS Similarity Distance
This algorithm allows you to determine a numeric distance between two given domains, using their WHOIS information.
This work is part of my master thesis and the soonest possible I going to add more theoric information and the experiments have been carried out for this algorithm.

## Authors
- **Raúl B. Netto** 
    ([@Piuliss](https://www.twitter.com/Piuliss), <raulbeni@gmail.com>, <rbenitez@uni.edu.py>, <benitrau@fit.cvut.cz>)

## Getting started
    
    git clone git@github.com:stratosphereips/whois-similarity-distance.git
    pip install -r requirements.txt
    python ./wsd_domains.py google.com cisco.com
    
## Optional
WSD scripts works with [pythonwhois](https://pypi.python.org/pypi/pythonwhois/2.4.3) library to get the 
WHOIS information of the domains. However, it is possible to use [passivetotal](https://pypi.python.org/pypi/passivetotal) library. 
It is the official library provided by the [RiskIQ](https://community.riskiq.com) community. 
For using *passivetotal* to get WHOIS information, you must have a account in [RiskIQ](https://community.riskiq.com)
and follow the next instructions:

    git clone git@github.com:stratosphereips/whois-similarity-distance.git
    pip install -r requirements.txt
    pt-config setup <USER-EMAIL> <USER-API-KEY>
    python ./wsd_domains.py google.com cisco.com -wl pt