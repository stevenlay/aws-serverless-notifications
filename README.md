<h1 align="center">Serverless Framework Notification Service</h1>
<p align="center">
  <i><strong>A modern, ES6-friendly Notification service ready for integration with Serverless Framework.</strong></i>
</p>

## Features

- Receive messages from another service
- Queue messages and reply to them in an arbitrary manner
- Send e-mails to specified addresses

## Getting started

### 1. Install dependencies

```sh
npm install
```

### 2. Change Configurations and Set Address

The initial batch size for the service is set to one. Please change it to whatever size you want, ideally greater than one.
The batch size will define how many requests are taken at once by AWS SQS to process.

Change the source address e-mail found within `src/handlers/sendMail.js` to a user defined one.

### 3. Deploy the stack

We need to deploy the stack in order to consume the private/public testing endpoints.

```sh
sls deploy -v
```
