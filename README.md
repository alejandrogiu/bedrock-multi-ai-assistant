# bedrock-multi-ai-assistant
A versatile Python-based AI assistant leveraging multiple Amazon Bedrock models for text generation, sentiment analysis, and image creation. Ideal for showcasing AWS AI integration skills.

# Multi-Model AI Assistant using Amazon Bedrock

## Project Overview

This project demonstrates a Python-based AI assistant that leverages multiple foundation models available through Amazon Bedrock. The assistant can perform various tasks such as text generation, sentiment analysis, and image generation, showcasing the versatility of AI models and their integration in a single application.

## Features

- Text Generation: Create original text content based on prompts.
- Sentiment Analysis: Analyze the sentiment of given text.
- Image Generation: Create images based on text descriptions.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.7 or higher installed
- An AWS account with access to Amazon Bedrock
- AWS CLI configured with appropriate credentials

## Setup

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/bedrock-ai-assistant.git
   cd bedrock-ai-assistant
   ```

2. Install the required Python packages:
   ```
   pip install boto3
   ```

3. Configure your AWS credentials if you haven't already:
   ```
   aws configure
   ```

4. Update the `model_id` parameters in the `BedrockAssistant` class methods to match the models available in your Amazon Bedrock account.

## Usage

To use the AI assistant, you can run the script directly or import the `BedrockAssistant` class into your own Python script.

### Running the script

```python
python bedrock_assistant.py
```

This will execute the example usage at the bottom of the script, demonstrating text generation, sentiment analysis, and image generation.

### Importing the class

```python
from bedrock_assistant import BedrockAssistant

assistant = BedrockAssistant()

# Generate text
text = assistant.generate_text("Write a short story about AI")
print("Generated Text:", text)

# Analyze sentiment
sentiment = assistant.analyze_sentiment("I love working with AI models!")
print("Sentiment Analysis:", sentiment)

# Generate image
image_base64 = assistant.generate_image("A futuristic city with flying cars")
print("Image generated (base64 string):", image_base64[:100] + "...")
```

## Customization

You can easily extend the `BedrockAssistant` class to include more functionality or use different models available through Amazon Bedrock. Simply add new methods to the class, following the pattern of existing methods.

## Contributing

Contributions to this project are welcome! Please fork the repository and submit a pull request with your improvements.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Amazon Web Services for providing the Bedrock service
- The AI community for developing the foundation models used in this project
