# Reflection Engine

A versatile Python-based tool for web interaction, Selenium automation, and AI-assisted task execution.

## Features

- 🤖 AI-powered command generation and execution
- 🌐 Web browsing and content retrieval
- 📷 Website screenshot capture
- 🔧 Custom Selenium code generation and execution
- 🚀 Interactive session with AI model
- 📊 Performance measurement for AI models

## Requirements

- Python 3.12
- Poetry (for dependency management)
- Chrome browser
- FFmpeg (for video clipping)

## Dependencies

Key dependencies include:
- selenium==4.25.0
- requests==2.32.3
- rich==13.8.1
- pillow==10.4.0
- validators==0.34.0
- webdriver-manager==4.0.2

For a full list of dependencies, see the `pyproject.toml` file.

## Installation

1. Clone this repository
2. Ensure you have Python 3.12 and Poetry installed
3. Install dependencies using Poetry:
   ```
   poetry install
   ```
4. Ensure Chrome and ChromeDriver are installed
5. Install FFmpeg for video clipping functionality

## Usage

Run the script in interactive mode:

```
poetry run python main.py -i --model llama3.2:3b
```

Available commands in interactive mode:
- `/cmd <prompt>`: Web interaction or custom Selenium code
- `/screenshot`: Take a screenshot of the last visited URL
- `/selenium <task>`: Generate custom Selenium code
- `/clip <input_file> <output_file> <start_time> <duration>`: Clip a video
- `exit`: Exit the session

## Advanced Usage

Customize system prompts:

```
poetry run python main.py -i --model llama3.2:3b --system-prompt-prefix "Your prefix here" --system-prompt-suffix "Your suffix here"
```

Measure AI model performance:

```
poetry run python main.py --model llama3.2:3b --prompt "Your prompt here"
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

MIT-ish

