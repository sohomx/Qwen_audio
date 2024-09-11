## This file implements a web-based application that performs the following functions:

1. Imports necessary libraries: transformers for the language model, gTTS for text-to-speech, torch for GPU support, and gradio for the user interface.
2. Sets up the Qwen2-1.5B-Instruct language model and tokenizer from Hugging Face.
3. Defines functions to process user input, generate responses, and convert text to speech:
- process_input(): Prepares prompts for translation or chat, generates responses using the language model.
- text_to_speech(): Converts the generated text to speech using gTTS.
- handle_interaction(): Combines the above functions to process user input and return text and audio outputs.


### Creates a Gradio interface with:

- Input: Text box for user input and dropdown for selecting action (translate to English/Chinese/Japanese or chat).
- Output: Text box for generated response and audio player for speech output.


Launches the Gradio interface, making it accessible via a public URL.

The application allows users to input text, choose an action (translation or chat), and receive both text and audio responses. It leverages the Qwen2-1.5B-Instruct model for natural language processing and gTTS for converting the generated text to speech in the appropriate language.
