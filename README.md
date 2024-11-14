# **Google reCAPTCHA Fully Requests Based Solver**

## Release

This project isn't fully finished right now, I need to train a lot more the AI. I'll let you know...

## Overview
This repository provides an advanced solution for solving Google's reCAPTCHA v2/v3. The system is designed for developers who need to bypass reCAPTCHA and BotGuard challenges in an automated, reliable, and efficient manner.

The solver works by mimicking real user interactions with reCAPTCHA services, bypassing security mechanisms using server-side requests and reverse-engineering techniques. This tool is particularly useful for automating tasks in environments where CAPTCHA protection is present, such as form submissions, web scraping, and automated testing.

⚠️ **Important:** This tool is intended for educational purposes only. Ensure that you comply with Google's Terms of Service and applicable laws before using it in any production or commercial environment.

---

## Features

- **Google reCAPTCHA v2 & v3 Solving**: Efficiently solve both reCAPTCHA v2 and reCAPTCHA v3 challenges using request-based mechanisms.
- **BotGuard Reverse Engineered Solver**: Bypass BotGuard protections that are designed to prevent bot traffic.
- **Easy Integration**: Provides a simple API for integrating CAPTCHA solving into your scripts or applications.
- **Automated Interaction Simulation**: Simulates human-like interaction to solve CAPTCHA challenges based on request analysis.
- **Request-based Solving**: Completely server-side and API-based, requiring no manual interaction.
- **Proxy Support**: Supports rotating proxies to avoid IP bans and to simulate multiple users.
- **High Success Rate**: Implements intelligent fallback mechanisms to increase the solving success rate for reCAPTCHA and BotGuard.

---

## Preview (video soon)

![image](https://github.com/user-attachments/assets/a650a163-b369-4065-8680-09c7b5afb023)



---


## Supported site

- [google.com](https://www.google.com/)
- [youtube.com](https://www.youtube.com/)
- [spotify.com](https://www.spotify.com/)
- [dev.to](https://www.dev.to/)
- Many more...

---

## Requirements

- **Windows 10** / **Windows 11** / **Linux** / **MacOS**
- **Python 3.10** or any modern version of Python.
- **Requests Library**: For making HTTP requests to interact with CAPTCHA services.
  
---

## Installation

To get started, simply clone the repository and install the required dependencies.

1. Clone this repository:

   ```bash
   git clone https://github.com/catcha8/recaptcha-solver.git
   cd recaptcha-solver
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```
## Usage

### Solving Google reCAPTCHA v2 & v3

1. **Initialize the solver**:

   ```python
   from recaptcha_solver import ReCaptchaSolver

   solver = ReCaptchaSolver(api_key="your_api_key")
   ```

2. **Solve a reCAPTCHA v2**:

   ```python
   response = solver.solve_recaptcha_v2(site_key="your_site_key", page_url="https://example.com")
   print("Captcha Response: ", response)
   ```

3. **Solve a reCAPTCHA v3**:

   ```python
   response = solver.solve_recaptcha_v3(site_key="your_site_key", page_url="https://example.com")
   print("Captcha Response: ", response)
   ```

## Configuration

This project uses an API key for CAPTCHA solving. You'll need to obtain an API key from [our CAPTCHA-solving service](https://discord.gg/XuGAPnAP45).

- Put your API key in the settings file (`config.json`).
- You can configure proxy settings in `config.json` too if you'd like to use rotating proxies.

---

## Advanced Features

- **Proxy Rotation**: Use rotating proxies to avoid IP bans.
- **Error Handling**: Robust error handling for failed CAPTCHA solving attempts.
- **Logging**: Detailed logs for debugging and monitoring solving attempts.
- **Captcha Timeout Management**: Handle timeouts and retries for CAPTCHA-solving.

---

## Contributing

Contributions to this project are welcome! If you'd like to improve the solver or add new features, feel free to fork the repository and submit a pull request.

### Steps to Contribute:

1. Fork this repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Make your changes and commit them (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Create a new Pull Request.

---

## Disclaimer

This project is **not affiliated** with Google or any CAPTCHA service. It is designed as a tool for educational purposes and should only be used responsibly. **Using this tool to circumvent CAPTCHA protections may violate the terms of service of various websites.** Always ensure you're in compliance with legal and ethical standards before using such tools.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Contact

For any questions, issues, or feature requests, feel free to open an issue or contact the maintainer at:

- **GitHub**: [catcha8](https://github.com/catcha8)
- **Discord**: [discord](https://discord.gg/XuGAPnAP45)

## Note for Google or BotGuard

Please read your emails...

## [More infos](https://dev.to/catcha8/recaptcha-reverse-engineering-9b0)


