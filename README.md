# FLUX.pro Image Generation API with Gradio Interface inside Google Colab enviroment

This project implements a Gradio interface for the FLUX.pro Image Generation API, allowing users to generate images from text prompts using Google Colab.

## Don't forget to use API KEY get one from https://api.bfl.ml/auth/login#

## Run in Google Colab

You can run this project directly in Google Colab without any local setup. Click the button below to open the notebook:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Y31u6I1Y7MG88VKOZeXdZLa_H4ovtgVl?usp=sharing)

## Usage Instructions

1. Click the "Open in Colab" button above to open the notebook in Google Colab.
2. In the Colab notebook, go to "Runtime" > "Run all" to execute all cells. This will:
   - Install the required packages
   - Set up the environment
   - Launch the Gradio interface
3. You will need to set your FLUX API key. Look for the cell that sets the API key and replace the placeholder with your actual key:
   ```python
   os.environ["BFL_API_KEY"] = "your-api-key-here"
   ```
4. After running all cells, you'll see a public URL for the Gradio interface. Click on this URL to open the interface in a new tab.
5. In the Gradio interface, enter a text prompt in the input box and click "Submit" to generate an image.

## Features

- Text-to-image generation using FLUX.pro API
- User-friendly Gradio interface
- Error handling and display
- Request tracking and logging
- Runs entirely in Google Colab - no local setup required

## Code Overview

The main components of the Colab notebook are:

1. Package Installation:
   - Installs `gradio`, `flux`, and other required packages.

2. API Setup:
   - Sets the FLUX API key as an environment variable.

3. Image Generation Function:
   - Defines `generate_image(prompt)` which sends requests to the FLUX API.

4. Gradio Interface:
   - Creates a simple UI for entering prompts and displaying generated images.

5. Error Handling:
   - Manages API errors, insufficient credits, and other exceptions.

6. Logging:
   - Tracks requests, completions, and errors for monitoring.

## Troubleshooting

- If you encounter an "Insufficient credits" error, check your FLUX API account balance.
- Ensure you've correctly set your API key in the notebook.
- If the Gradio interface doesn't appear, try rerunning the cells in the notebook.

## License

This project is licensed under the MIT License. This means:

- You are free to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the software.
- The software is provided "as is", without warranty of any kind, express or implied.
- The authors or copyright holders are not liable for any claim, damages or other liability arising from the use of the software.

---

For more information on the FLUX.pro API, visit [https://api.bfl.ml](https://api.bfl.ml).
