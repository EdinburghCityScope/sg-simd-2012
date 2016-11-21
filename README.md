# sg-simd-2012
##The Scottish Index of Multiple Deprivation 2004-2012

The Scottish Index of Multiple Deprivation (SIMD) provides a relative ranking of the Data Zones in Scotland from 1 (most deprived) to 6505 (least deprived) based on a weighted combination of data in the domains of Income, Housing, Health, Education, Skills and Training, Employment, Geographic Access to Services, and Crime (no Crime data available for SIMD 2004).

Each of the domains can also be ranked individually. Using the relative rankings each data zone can be assigned to a decile for each domain and the overall index. Decile 1 is the most deprived 10% of Data Zones and decile 10 is the least deprived 10% of Data Zones. When comparing results from the different versions of the SIMD it is important to take into account changes to the methodology used to construct the individual domains and the overall SIMD between the three indices. More information can be found at [www.scotland.gov.uk/simd](http://www.scotland.gov.uk/simd).

You can also view a map of [SIMD](http://statistics.gov.scot/slice?dataset=http%3A%2F%2Fstatistics.gov.scot%2Fdata%2Fscottish-index-multiple-deprivation&http%3A%2F%2Fpurl.org%2Flinked-data%2Fcube%23measureType=http%3A%2F%2Fstatistics.gov.scot%2Fdef%2Fmeasure-properties%2Fdecile&http%3A%2F%2Fpurl.org%2Flinked-data%2Fsdmx%2F2009%2Fdimension%23refPeriod=http%3A%2F%2Freference.data.gov.uk%2Fid%2Fyear%2F2012&http%3A%2F%2Fstatistics.gov.scot%2Fdef%2Fdimension%2FsimdDomain=http%3A%2F%2Fstatistics.gov.scot%2Fdef%2Fconcept%2Fsimd-domain%2Fsimd&tab=charts).

## License

Data is licensed under the Open Government License: http://www.nationalarchives.gov.uk/doc/open-government-licence/version/2/

## Requirements

- NodeJS
- npm

## Installation

Clone the repository

```
git clone https://github.com/EdinburghCityScope/sg-simd-2012.git
```

Install npm dependencies

```
cd sg-simd-2012
npm install
```

Run the API (from the sg-simd-2012 directory)

```
node .
```

Converting the extracted data into loopback data.

```
node scripts/featureCollectionToLoopbackJson.js
```

Re-build data files from the statistics.gov.scot API

```
node scripts/build-data.js
```
