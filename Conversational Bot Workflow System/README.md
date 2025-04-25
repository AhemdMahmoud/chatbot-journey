# ConvoBot - Conversational Bot Workflow System



# US Data Explorer Bot - Botpress Project

## Project Overview
This Botpress-powered chatbot allows users to explore data through a conversational interface. The bot currently features two main workflows: retrieving USA population data by year and displaying random dog images. Built with Botpress's visual flow editor, this project demonstrates how to create a user-friendly bot with API integrations and input validation.

![image](https://github.com/user-attachments/assets/b6ed7496-6efc-42f9-bbcf-61feec8c2c02)
![image](https://github.com/user-attachments/assets/70f35355-95c6-49b8-8c2e-66bc6fff528b)


## Bot Capabilities
- Greets users and offers data exploration options
- Retrieves and displays USA population statistics by year
- Shows random dog images on request
- Validates user inputs
- Handles errors gracefully with custom messages

## Workflow Structure

### Main Flow
- **Entry Point**: The conversation begins here
- **Say-hello Node**: Introduces the bot and its capabilities
- **Choice Node**: Presents users with options to explore USA population data or view random dog images

### USA Population Flow
- **API Call Node**: Makes requests to a population data API
- **print-us-population Node**: Formats and displays population data
- **validator-year Node**: Ensures year inputs are valid
- **warning-message Node**: Displays when invalid years are entered
- **error-fetch-pop Node**: Handles API errors

### Random Dog Image Flow
- **Entry Point**: Simple flow to fetch and display dog images
- **End of Workflow Node**: Returns users to previous conversation

## Setup Instructions

### Prerequisites
- Botpress account
- Node.js installed (for local development)

### Installation
1. Clone this repository
2. Import the bot into Botpress:
   - Open Botpress Studio
   - Click "Import Bot"
   - Select the bot files from this project
3. Configure API credentials in the bot's global variables

### Configuration
The bot requires configuration for:
- Population data API endpoint
- Dog image API service
- Any authentication tokens needed for the APIs

## Testing the Bot
1. Use the Botpress Emulator to test conversations
2. Try different paths:
   - Request USA population data for various years
   - Test input validation with invalid years
   - Request random dog images

## Customization
This bot can be extended with additional features:
- More data visualization options
- Additional API integrations
- Enhanced error handling
- User preference storage

## Deployment
The bot can be deployed to:
- Botpress Cloud
- Custom server with Botpress runtime
- Integration with messaging platforms (Facebook, Slack, etc.)

## Bot Structure
```
flows/
├── main.flow.json
├── error-handling.flow.json  
├── usa-population-flow.flow.json
└── random-dog-image.flow.json
actions/
├── fetchPopulationData.js
└── getRandomDogImage.js
intents/
└── data-requests.json
content/
└── greeting-messages.json
```
