# Chatbot Project

A flexible and customizable chatbot implementation built with response templates and conversational capabilities.

## Project Overview

This project implements a conversational chatbot with customizable response templates. The chatbot can handle various user inputs, display interactive cards, and maintain contextual conversations.

## Features

- Custom response templates
- Interactive card interfaces
- File sharing capabilities
- GitHub integration
- Support for multiple conversation flows
- Customizable greeting messages
- Image handling and display

## Response Templates

The chatbot uses predefined templates to structure responses. Below are examples of our templates:

### Template Examples

<!-- Option 1: Use raw GitHub URLs (works if repository is public) -->
![Template Example 1](https://raw.githubusercontent.com/AhemdMahmoud/chatbot-journey/main/response%20templates/Screenshot%202025-04-26%20105509.png)
![Template Example 2](https://raw.githubusercontent.com/AhemdMahmoud/chatbot-journey/main/response%20templates/Screenshot%202025-04-26%20105605.png)
![Template Example 3](https://raw.githubusercontent.com/AhemdMahmoud/chatbot-journey/main/response%20templates/Screenshot%202025-04-26%20105639.png)

<!-- Option 2: Use relative paths (if images are in the same repository) -->
<!-- 
![Template Example 1](./response%20templates/Screenshot%202025-04-26%20105509.png)
![Template Example 2](./response%20templates/Screenshot%202025-04-26%20105605.png)
![Template Example 3](./response%20templates/Screenshot%202025-04-26%20105639.png)
-->

### Card Template
```json
{
  "type": "card",
  "content": {
    "title": "Welcome ya bro",
    "subtitle": "i hope you are well",
    "actions": [
      {
        "text": "say hello",
        "action": "RESPONSE"
      },
      {
        "text": "go to your github",
        "action": "LINK",
        "url": "https://github.com/username/repository"
      },
      {
        "text": "please postback again",
        "action": "POSTBACK"
      }
    ]
  }
}
```

### Text Response Template
```json
{
  "type": "text",
  "content": "Hello ya sahpy"
}
```

### Image Response Template
```json
{
  "type": "image",
  "url": "image_url.jpg",
  "caption": "your image"
}
```

### File Response Template
```json
{
  "type": "file",
  "name": "Acpc problem set",
  "action": "DOWNLOAD"
}
```
