# Automated-ML-Notifications

Get notified of a custom event via text message

## Installation

Choose your preferred package manager for installing dependencies:

### Using pnpm

```bash
pnpm install
```

### Using npm

```bash
npm install
```

### Using Yarn

```bash
yarn
```

### Using Bun

```bash
bun install
```

## Setting Up Twilio WhatsApp Sandbox

1. Join the sandbox following this link: [Twilio WhatsApp Sandbox](https://console.twilio.com/us1/develop/sms/try-it-out/whatsapp-learn).
2. Use your real WhatsApp number as this number will be used as the "to" in the message creation.

## Configuring Environment Variables

Create a `.env` file at the root of your project and write your Twilio credentials and phone numbers in it:

```env
TWILIO_ACCOUNT_SID=<Your Twilio Account SID>
TWILIO_AUTH_TOKEN=<Your Twilio Auth Token>
TO_NUMBER="whatsapp:<Your WhatsApp Number>"
FROM_NUMBER="whatsapp:<Your Twilio WhatsApp Number>"
```

You can find these values through the links in the Useful Links section below.

## Running the Script

Run the script using your package manager. Here's how you can do it with pnpm, but you can use any package manager:

```bash
pnpm run send
```

Alternatively, if using Bun:

```bash
bun src/index.ts
```

## Useful Links

- [WhatsApp Sandbox](https://console.twilio.com/us1/develop/sms/try-it-out/whatsapp-learn): Where you will get the FROM number.
- [Twilio SMS Overview](https://console.twilio.com/us1/develop/sms/overview): For a general overview of Twilio SMS services.
- [Twilio Console](https://console.twilio.com/): To get your account/auth token/TO phone number. These will be located at the bottom under "Account Info".
