# ConvoBot - Conversational Bot Workflow System

## Project Overview
ConvoBot is a visual workflow management system for building conversational bots. It allows you to create, manage, and deploy interactive chatbot experiences without extensive coding knowledge. The system uses a node-based interface where you can design conversation flows, handle user inputs, make API calls, and provide dynamic responses.
![image](https://github.com/user-attachments/assets/b6ed7496-6efc-42f9-bbcf-61feec8c2c02)

## Key Features
- **Visual Workflow Editor**: Design conversation flows using an intuitive drag-and-drop interface
- **Multiple Flow Support**: Create and manage separate conversation flows (Main, Error handling, etc.)
- **Conditional Branching**: Route conversations based on user input and validation
- **API Integration**: Connect to external services like population data APIs and image generators
- **Input Validation**: Verify user inputs with custom validation rules
- **Error Handling**: Create dedicated flows for gracefully managing errors

## Workflow Components

### Main Flow
The main flow begins with a welcome message and branches into different paths based on user choices:
- **Say-hello**: Initial greeting and interaction with the user
- **Choice Node**: Allows users to select between USA population data or random dog images
- **API Call**: Makes external API requests for data retrieval
- **Validator**: Validates user inputs (e.g., year validation)

### USA Population Flow
This flow handles retrieving and displaying USA population data:
- Fetches population data for a specified year
- Displays formatted population information
- Handles API errors with appropriate messaging
- Provides validation for year input

### Random Dog Image Flow
This flow manages the retrieval and display of random dog images:
- Connects to a dog image API
- Displays random dog images to the user
- Offers options to view additional images

### Error Handling
The system includes dedicated error handling for various scenarios:
- Invalid inputs
- Failed API calls
- Timeout errors
- General system errors

## Getting Started
1. Clone the repository
2. Install dependencies
3. Run the development server
4. Access the workflow editor at http://localhost:3000

## Project Structure
```
convobot/
├── src/
│   ├── components/
│   │   ├── nodes/
│   │   ├── workflows/
│   │   └── editor/
│   ├── services/
│   │   ├── api/
│   │   └── validators/
│   └── utils/
├── public/
└── docs/
```

## Configuration
The system can be configured through the `config.json` file to adjust:
- API endpoints
- Validation rules
- UI appearance
- Response templates

## Deployment
The workflow can be deployed as:
- A standalone web application
- An embedded widget for websites
- A service for integration with messaging platforms

## Contributing
Contributions are welcome! Please see our contributing guidelines for more details.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
