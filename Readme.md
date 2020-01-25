# Parsing Swissmedic and Pharmnet with Meteor

#### Install Meteor on Linux
`curl https://install.meteor.com/ | sh`

#### Install dependencies
$ meteor npm install

#### Run GUI at localhost:3000 with pharmnet data
$ meteor --once --settings pharma.json

#### Import HPC, DHPC and Chargenrückrufe from Swissmedic.ch
$ meteor --once --settings swissmedic.json

#### Import from Pharmnet
$ meteor --once --settings atc.json   


### Import from drugshortage

$ meteor --settings drugshortage.json --once


### Import from pei.de
$ meteor --settings pei.json  --once



#### Check files
$ cd public/exports

#### Check files in Browser
Open http://localhost:3000 in the browser

#### Debugging
$ METEOR_PROFILE=1 METEOR_LOG=debug meteor --verbose

### Missing ATC-Code
./atc.json

set "loadMissing":true
set "Missing" => Missing code in array

### Convert json2csv
/home/zeno/.nvm/versions/node/v11.12.0/bin/json2csv
