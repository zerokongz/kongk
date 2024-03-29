# nfp-YAYAML
Yet Another Yet Another Markup Language


Installation
npm install yayaml

Usage
var parseYayaml = require("yayaml");
var myObject = parseYayaml(fs.readFileSync("myfile.yay", "utf8"));

Testing
npm test

What is YAYAML language?
YAYAML is a very light spin on YAML, designed to create a visually unopinionated configuration language. Bonus points: the file extension gets to be ..yay


Example
node api-service-http-frontend
    title   API Server HTTP Frontend 02
    region  ap-southeast2
    region  api
    region  HTTP Frontend
    type    web
    owner   John Smith <john.smith@example.com>
    tag     UAT
    tag     API
    tag     HTTP
    tag     web
    tag     smithj
    depends api-service-cache
    depends api-service-elasticsearch
    depends ops-dmz-proxy
    
    metric messages_received
        weight  1
        top
            acceptable  500
            critical    1000
        bottom
            acceptable  25
            critical    5
