# AI Ad Creative Generator

A **generative AI** web app that creates **Meta (Facebook and Instagram) ad creatives** from a short idea. It writes the ad copy with an **LLM** (Groq), generates the image with an **AI image model** (fal.ai), and stamps your logo on the result. It is built with Python and Streamlit, and exports ready-to-post **Feed** and **Story** formats.

## Features

- **Ad ideas from a topic:** describe your product or message and generate headline, subtext and call-to-action options
- **Auto Detect or Manual settings:** the app detects the ad phase (problem, solution, results), topic category, background and emotion, or you set them yourself
- **Editable copy and prompt:** change the headline, subtext, CTA, font and layout, then rebuild the image prompt
- **Two formats:** Feed (1080×1080) and Story (1080×1920), each with a regenerate option and a download button
- **Logo stamping:** your `logo.png` is added to every generated creative
- **Chat assistant:** ask for headline ideas or change the image direction in plain language
- **Login:** user authentication with `streamlit-authenticator`
- **Activity and feedback logging:** actions are logged to a Google Sheet, and feedback on each creative can be saved
- **Credit check:** shows your remaining fal.ai credits in the sidebar

## Keywords

Generative AI · LLM · Prompt engineering · AI image generation · Ad creative automation · Marketing automation · Meta Ads · Facebook Ads · Instagram Ads · Streamlit · Python

## Tech Stack

- Python and [Streamlit](https://streamlit.io/)
- [Groq](https://groq.com/) API for ad copy and the chat assistant
- [fal.ai](https://fal.ai/) for image generation (`fal-ai/nano-banana-2`, with its `edit` variant)
- Pillow for image processing and logo stamping
- Google Sheets (service account) for activity logs
- `streamlit-authenticator` and `bcrypt` for login

## Project Structure

| Path | Purpose |
| :--- | :--- |
| `app.py` | The Streamlit app: UI, prompt building, image generation and logging |
| `logo.png` | Logo stamped on generated creatives |
| `requirements.txt` | Python dependencies |
| `.streamlit/secrets.toml.example` | Template for the secrets file |
| `.devcontainer/` | Dev container configuration |

## Author

**Amar Chaurasiya**, open to full-time roles and freelance work.

- Email: [amarchaurasiya124@gmail.com](mailto:amarchaurasiya124@gmail.com)
- LinkedIn: [amar-chaurasiya-163788262](https://www.linkedin.com/in/amar-chaurasiya-163788262)
- Portfolio: [amarchaurasiya.vercel.app](https://amarchaurasiya.vercel.app)
