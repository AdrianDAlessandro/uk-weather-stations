# Cleaning Weather Station Records

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/ImperialCollegeLondon/uk-weather-stations?quickstart=1)

This repository is the starting point for the Cleaning Weather Station Records project in the ECRI Research Computing and Data Science hackathon. The project instructions are on the [hackathon wiki](https://github.com/ImperialCollegeLondon/prices/wiki/Projects).

## Quickstart

Open a Codespace with the button above, which has everything set up already. Or, with Python 3.10 or later and Git:

```bash
git clone https://github.com/ImperialCollegeLondon/uk-weather-stations.git
cd uk-weather-stations
python -m venv .venv
source .venv/bin/activate
python -m pip install -e ".[dev]"
```

## Data

The folder `data/raw` contains the monthly records for eight UK weather stations, downloaded from the Met Office's [historic station data](https://www.metoffice.gov.uk/research/climate/maps-and-data/historic-station-data) page on 20 October 2026.

| File | Station |
|---|---|
| `braemardata.txt` | Braemar |
| `cambridgedata.txt` | Cambridge NIAB |
| `eskdalemuirdata.txt` | Eskdalemuir |
| `heathrowdata.txt` | Heathrow |
| `lerwickdata.txt` | Lerwick |
| `lowestoftdata.txt` | Lowestoft |
| `oxforddata.txt` | Oxford |
| `southamptondata.txt` | Southampton |

Each file starts with a few lines about the station, followed by one line for each month:

| Column | Meaning |
|---|---|
| `yyyy`, `mm` | Year and month |
| `tmax` | Mean daily maximum temperature (°C) |
| `tmin` | Mean daily minimum temperature (°C) |
| `af` | Days of air frost |
| `rain` | Total rainfall (mm) |
| `sun` | Total sunshine (hours) |

Contains public sector information licensed under the [Open Government Licence v3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/).
