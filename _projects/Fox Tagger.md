---
name: Fox Tagger
tools: [MetaMask Snaps, React, TypeScript, Gatsby.js]
image: https://images.ctfassets.net/clixtyxoaeas/2rCBWZUhCIH3Ws6APjjIpL/1703354ceb197ccb931b118de1acf08f/Snaps_Spotlights_Feature_Images.png
description: A MetaMask Snap extension that helps users track and manage their crypto expenditure through smart tagging and usage analytics.
---

# Fox Tagger

## An Intelligent Transaction Management Snap for MetaMask

Fox Tagger is a powerful MetaMask Snap extension designed to revolutionize how users track and manage their cryptocurrency transactions. By enabling users to tag wallet addresses and monitor their expenditures, it provides comprehensive analytics and alerts to help users maintain better control over their crypto spending.

{% include elements/figure.html image="https://images.ctfassets.net/clixtyxoaeas/af97fa66d05c055d5988345d/91a81091be18ced0fffb9b337cc6c436/Screenshot_2023-05-10_at_1.17.17_PM" caption="Fox Tagger Team at work" %}

## Motivation

With the exponential growth in cryptocurrency adoption through MetaMask, users need better tools to track and organize their transactions. Fox Tagger addresses this need by providing a powerful tagging system that helps users:

- Track expenditure patterns through customizable tags
- Set spending limits and receive alerts
- Monitor transaction history with detailed analytics
- Make informed decisions about their crypto spending

## Technical Implementation

### Architecture
The project consists of two main components:
1. **MetaMask Snap Backend**: Handles core functionality using the Snaps API
2. **Gatsby.js Frontend**: Provides the user interface and companion DApp

### Key Features
- **Persistence Storage**: Maintains user tags and transaction data
- **Smart Notifications**: Alerts users about spending limits and transaction updates
- **Cron Jobs**: Automated monitoring and reporting of transaction patterns
- **Transaction Insights**: Real-time analysis and visualization of spending patterns
- **XMTP Protocol**: Enables secure user-to-user payment requests

### Data Structure
```json
{
  "from_account0": {
    "mainMapping": {
      "to_account0": ["tag0", "tag1"]
    },
    "usage": {
      "tag0": {
        "limit": "100000000000",
        "used": "800000",
        "notified": false
      }
    },
    "latestHash": "transaction_hash0"
  }
}
```

## Key Features

### Tag Management
- Create and manage custom tags for different addresses
- Organize transactions by categories
- Track spending patterns by tag

### Analytics Dashboard
- Visual representation of spending by category
- Historical transaction analysis
- Usage trends and patterns

### Smart Alerts
- Custom spending limit notifications
- Weekly summary reports
- Transaction insights and warnings

### Payment Requests
- Direct ETH amount requests between users
- XMTP protocol integration for secure messaging
- Real-time notification system

## Technology Stack

### Frontend
- Gatsby.js for the web interface
- React for component architecture
- TypeScript for type safety
- Chart.js for analytics visualization

### Backend
- MetaMask Snaps API
- XMTP Protocol for messaging
- Etherscan API integration
- Smart persistent storage system

## Future Enhancements

The project roadmap includes several exciting features:
- Machine Learning models for spending prediction
- Enhanced analytics and visualization
- Multi-chain support beyond Goerli Testnet
- Transaction splitting functionality
- Custom UI improvements using new Snap features

## Links

{% include elements/button.html link="https://github.com/shree675/FoxTagger" text="View on GitHub" icon="fab fa-github" %}
