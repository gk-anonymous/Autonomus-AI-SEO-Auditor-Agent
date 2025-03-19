# Autonomus-AI-SEO-Auditor-Agent

## Project Overview
This project is an AI-powered chatbot that analyzes SEO performance for a given website. It utilizes OpenAI's GPT-4 model to process user queries and perform SEO audits using the RapidAPI SEO Analyzer. The chatbot runs in a loop, making decisions based on available actions and generating structured responses.

## Features
- Uses OpenAI's GPT-4 for intelligent query processing
- Performs SEO audits for websites using RapidAPI
- Extracts structured JSON responses for function execution
- Iteratively refines results with multiple query loops

## File Structure
```
├── action.py                # Contains the function to fetch SEO reports
├── chatbit_agent.py         # Chatbot implementation with function calling mechanism
├── main.py                  # Main script that runs the chatbot loop
├── prompt.py                # Contains system prompt definitions for structured interactions
```

## Installation & Setup
### Prerequisites
- Python 3.8+
- OpenAI API Key
- RapidAPI Key

### Installation Steps
1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/seo-chatbot.git
   cd seo-chatbot
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Configure API keys:
   - Add your OpenAI and RapidAPI credentials in the respective files or environment variables.

## Usage
1. Run the chatbot:
   ```sh
   python chatbit_agent.py
   ```
2. Enter website-related queries like:
   ```
   how many images without alt tags are there on learnwithhasan.com
   ```
3. The chatbot will analyze the website and return an SEO report.

## How It Works
1. The chatbot initializes with a system prompt.
2. It processes user queries using GPT-4.
3. It identifies whether an SEO action needs to be executed.
4. Calls the `get_seo_page_report` function via RapidAPI.
5. Returns a structured response with relevant SEO insights.

## Example Interaction
```
User: how many images without alt tags are there on learnwithhasan.com?
Bot: Generating SEO report...
Bot: Action_Response: {'images_without_alt': 5}
Bot: Answer: There are 5 images without alt tags on learnwithhasan.com.
```

## License
This project is licensed under the MIT License.

## Author
Developed by [Your Name] 🚀

