# AWSLambda Twilio Outbound SIP TwiML [![Build Status](https://travis-ci.org/chriselsen/AWSLambda_Twilio_SipOutbound.svg?branch=master)](https://travis-ci.org/chriselsen/AWSLambda_Twilio_SipOutbound)
AWS Lambda Function to create a Twilio TwiML response for usage with [Outbound SIP](https://www.twilio.com/docs/api/twilio-sip/pv-sip-registration), together with AWS API Gateway.

Pre-Requisites:
* API Gateway with [Lambda Proxy integration](http://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-create-api-as-simple-proxy-for-lambda.html#api-gateway-create-api-as-simple-proxy-for-lambda-build)
* Twilio account and [SIP registration](https://www.twilio.com/docs/api/twilio-sip/pv-sip-registration)

Usage:
* In Twilio (Home / Voice / SIP Domains / Domains /) use the following "Request URL" as "HTTP POST":
  * https://myapiid.execute-api.us-east-1.amazonaws.com/prod/SIP_Outbound?callerId=14155551234
