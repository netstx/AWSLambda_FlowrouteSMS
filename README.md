# AWSLambdaFlowrouteSMS [![Build Status](https://travis-ci.org/chriselsen/AWSLambda_FlowrouteSMS.svg?branch=master)](https://travis-ci.org/chriselsen/AWSLambda_FlowrouteSMS)
AWS Lambda Function to process Flowroute text messages.
Refer to https://wp.me/p3w6wb-A0 for more information

Pre-Requisites:
* Amazon SES setup and domain or e-mail authenticated
* Role for Lambda that allows access to Amazon SES

Flowroute API versions:
* Flowroute's API v2.0 posted a single JSON string to the callback URL. Since v2.1, it's now a nested JSON string (data.attributes.xyz). This fork has fixed JSON parsing and a PR was sent to the original project.
