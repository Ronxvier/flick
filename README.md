
# flick  
**AI-powered terminal assistant for natural language project scaffolding and coding.**  
Built for macOS · Powered by Google Gemini · Written in Python

---

## What is flick?

**flick** is a minimal AI assistant that runs in your macOS terminal. It uses natural language input to help you generate code, scaffold new projects, and streamline development tasks — all without leaving the command line.

---

## What can flick do?


https://github.com/user-attachments/assets/92f21fa0-504b-4997-84b2-adf37a9f0022


- Initialize and build new projects using natural language  
- Generate and refactor code in real time  
- Summarize output, errors, or logs  
- Suggest terminal commands and scripting solutions  

---

## Installation

### Requirements

- macOS  
- Python 3.12+  
- Google Gemini API key (free from [Google AI Studio](https://makersuite.google.com/))

### Setup Steps

1. Clone the repo  

2. Set up the virtual environment  
   ```bash
   cd flick
   python3 -m venv flickvenv
   source flickvenv/bin/activate
   pip install -q -U google-genai
   pip install "urllib3<2.0" # (optional, but may prevent warnings)
   ```

3. Get your Python path  
   ```bash
   which python
   ```
   Copy that path.

4. Deactivate the environment  
   ```bash
   deactivate
   ```

5. Install flick  
   - Unzip the repo if needed.  
   - Move the `flick` file to your local bin:  
     ```bash
     mv flick /usr/local/bin/ # (if this directory does not exist, you may need to create it.)
     ```
   - Navigate to the install location:  
     ```bash
     cd /
     cd usr/local/bin/
     ```
   - Open `flick` in your preferred terminal editor:  
     ```bash
     nvim flick # nano or vim works too
     ```
   - Replace:  
     - `YOUR/PATH/GOES/HERE` with the Python path you copied. **Note:**(The '#!' at the beginning of the path is **necessary.**)
     - `YOUR-KEY-GOES-HERE` with your Gemini API key (inside the quotes)

6. Make it executable  
   ```bash
   chmod +x flick
   ```

7. You can now run `flick` from anywhere in your terminal.

---

## Example usage

```bash
flick create a new python project with a virtual environment and main.py
```

---

## License

MIT – use it freely, modify as needed.

