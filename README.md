# Terminal Chatbot

This is a simple terminal-based chatbot built using Hugging Face's `transformers` library. It utilizes the [facebook/blenderbot-400M-distill](https://huggingface.co/facebook/blenderbot-400M-distill) pre-trained conversational model.

## Features

- **Conversational AI**: Uses BlenderBot, a powerful conversational model by Facebook AI.
- **Terminal Interface**: Interact with the chatbot directly from your terminal.
- **Contextual Memory**: Maintains a history of your conversation for more coherent responses.

## Requirements

- Python 3.6 or above
- [transformers](https://pypi.org/project/transformers/)
- [torch](https://pypi.org/project/torch/)

## Installation

First, clone this repository or download the `chatbot.py` file.

Install the required dependencies:

```bash
pip install transformers torch
```

## Usage

Run the chatbot script in your terminal:

```bash
python chatbot.py
```

Type your messages after the `>` prompt. The bot will respond, and the conversation will continue until you manually exit (e.g., with `Ctrl+C`).

## Example

```
> Hello!
Hello! How can I help you today?
> Tell me a joke.
Why did the scarecrow win an award? Because he was outstanding in his field!
```

## Notes

- The first time you run the script, the model weights will be downloaded. This may take a few minutes depending on your internet speed.
- The script maintains the full conversation history for context, which may slow down long sessions.

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgements

- [Hugging Face Transformers](https://huggingface.co/transformers/)
- [Facebook BlenderBot](https://huggingface.co/facebook/blenderbot-400M-distill)
