# FLUX.pro Image Generation API with Gradio Interface

This project implements a Gradio interface for the FLUX.pro Image Generation API, allowing users to generate images from text prompts.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Configuration](#configuration)
- [Error Handling](#error-handling)
- [Logging](#logging)
- [Contributing](#contributing)
- [License](#license)

## Installation

To set up this project, follow these steps:
Install the required packages:
   ```
   pip install gradio
   pip install git+https://github.com/black-forest-labs/flux.git
   pip install requests Pillow
   ```

## Usage

To run the application:

1. Set your FLUX API key as an environment variable:
   ```
   export BFL_API_KEY="your-api-key-here"
   Signup and get API KEY from this link https://blackforestlabs.ai/
   ```

2. Run the Python script:
   ```
   python [script_name].py
   ```

3. Open the Gradio interface in your web browser using the provided URL.

4. Enter a text prompt in the input box and click "Submit" to generate an image.

## Features

- Text-to-image generation using FLUX.pro API
- User-friendly Gradio interface
- Error handling and display
- Request tracking and logging

## Configuration

The script uses the following configuration:

- FLUX API Key: Set as an environment variable `BFL_API_KEY`
- FLUX Model: "flux.1.1-pro"
- Logging Level: INFO

## Error Handling

The script includes error handling for:
- API errors
- Insufficient credits
- General exceptions

Error messages are displayed in the Gradio interface and logged.

## Logging

The script uses Python's `logging` module to log:
- Request processing
- Successful completions
- Errors
- Keep-alive messages

## Contributing

Contributions to this project are welcome. Please follow these steps:

1. Fork the repository
2. Create a new branch
3. Make your changes and commit them
4. Push to your fork and submit a pull request


---

For more information on the FLUX.pro API, visit [https://api.bfl.ml](https://api.bfl.ml).
