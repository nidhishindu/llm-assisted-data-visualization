# llm-assisted-data-visualization
An LLM-assisted data visualization workflow demonstrating an agentic loop where AI generates, executes, critiques, and refines Python code to analyze a coffee sales dataset.

This project explores how Large Language Models (LLMs) can support real-world data analysis through an agentic workflow, showcasing how AI can collaborate with analysts to speed up insights rather than replace them.

The project is based on an ungraded lab from DeepLearning.AI, adapted, debugged, and executed locally with improvements added throughout.

🔍 Project Overview

The goal of this project is to implement an LLM-driven loop that:

Generates plotting code using an LLM

Executes that code to produce a chart

Critiques the generated chart using a vision-enabled LLM

Refines the code and regenerates an improved visualization

This “generate → execute → critique → refine” cycle demonstrates how agentic AI patterns can support analytical workflows—enhancing iteration speed, improving visualization quality, and reducing repetitive manual work.

📊 Dataset

The dataset represents coffee machine sales and includes fields such as:

date

time

price

cash_type

coffee_name

month

quarter

year

If this dataset originated from the DeepLearning.AI lab environment, please follow their usage terms.

🧠 What I Learned & Contributed

Although the project framework comes from DeepLearning.AI, I completed the lab independently and expanded on it through:

✔️ Local debugging

Fixed execution issues in the notebook

Adjusted environment configuration

Repaired broken imports and paths

Ensured charts saved correctly without plt.show()

✔️ Secure API key handling

Set up .env file for private API keys

Loaded environment variables safely using python-dotenv

Avoided exposing credentials in code or version control

Added .env.example for safe sharing

✔️ LLM workflow integration

Ran the full agentic loop end-to-end

Passed charts to a vision-enabled LLM for visual critique

Parsed and executed LLM-generated code from <execute_python> tags

Compared and analyzed improvements between V1 and V2 charts

✔️ Cost awareness

While experimenting, I became familiar with responsible token usage—an important real-world consideration when integrating LLMs into analytical workflows.

✔️ Analytical perspective

As a full-time data analyst, my goal wasn’t to automate my role, but to explore how AI can enhance everyday analysis:

Faster prototyping

Clearer visualizations

Reduced repetitive work

Smarter iteration loops

This project reflects my curiosity about how LLMs can be integrated meaningfully into modern analytical environments.

🗂️ Repo Structure
llm-coffee-visualization/
│
├─ M2_UGL_1.ipynb           # Main notebook
├─ M2_UGL_1.html            # Clean preview for recruiters
├─ utils.py                 # Helper functions (LLM calls, image encoding, etc.)
│
├─ charts/
│   ├─ chart_v1.png
│   └─ chart_v2.png
│
├─ .env.example             # Safe template for API environment variables
├─ requirements.txt         # Project dependencies
├─ README.md                # You're reading this :)
└─ .gitignore               # Secrets, checkpoints, and venv excluded

🚀 How to Run the Project Locally
1. Clone the repository
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>

2. Set up a virtual environment (recommended)
python3 -m venv venv
source venv/bin/activate     # macOS / Linux
# .\venv\Scripts\activate     # Windows

3. Install dependencies
pip install -r requirements.txt

4. Create a .env file
OPENAI_API_KEY=your_key_here

5. Launch Jupyter Notebook
Jupyter Notebook M2_UGL_1.ipynb

📝 Attribution

This project is based on an ungraded lab from DeepLearning.AI.
All datasets, starter materials, and instructional content belong to the original creators.

I completed, debugged, and extended the project for learning and portfolio purposes, with full credit to DeepLearning.AI.

🤝 Acknowledgements

DeepLearning.AI — for designing the original lab and providing the dataset.

The open-source libraries powering this project: pandas, matplotlib, python-dotenv, and more.

The broader AI community for inspiring curiosity around agentic patterns.

⭐ Final Note

This project helped me explore how AI can integrate into practical analytical workflows—not as a replacement, but as a powerful collaborator.

If you have suggestions or want to discuss LLM-powered analytics, feel free to connect!
