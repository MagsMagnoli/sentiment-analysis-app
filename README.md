# Sentiment Analysis App

A premium sentiment analysis application that makes use of the following:

- Authentication with firebase
- Paywall with stripe
- Sentiment analysis on text with Google's Cloud Natural Language library
- Hosting with firebase
- React frontend
- Firebase functions backend

## Getting Started

- Create firebase project
- Enable billing in order to use non-Google services
- Install firebase cli tools
- Clone repo and configure to use your firebase project via cli
- Install dependencies in `functions` via `npm install`
- Create stripe account
- Set stripe secret to cloud functions via `firebase functions:config:set stripe.token=<YOUR TOKEN>`
- Set stripe publishable key in `config.ts`
- Deploy functions via `firebase deploy --only functions`
- Deploy firestore rules via `firebase deploy --only rules`
- Set firebase function URLs in `config.ts`
- Deploy app using `firebase deploy --only hosting`
- Test stripe integration on site via `firebase open hosting:site`
