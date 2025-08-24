
# setup 
Prereqs
- Python 3.11 or higher 
- uv (optional)

Steps 

1) create venv and install dependencies 
# WITH UV 
uv venv .venv
source .venv/bin/activate
uv pip install -r requirements.txt

Issue with UV - pulling x86_64 wheels for pydantic_core 
- incompatible with arm (apple silicon)

# WITH PIP 
python -m venv pip_venv 
source pip_venv/bin_activate 
pip install -r requirements.txt

2) create .env file 
touch .env 
add TAVILY_API_KEY="your_api_key"

# Learning 

1) clone repo 
2) pull the hello world commit (first commit)
3) run: python test.py 
4) follow the print statements to see the agent workflow and how it passes data to itself!  