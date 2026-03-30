# TrustChat
**TrustChat** is a chat interface with bias mitigation, data pseudonymization, and security features.

## Setup
```bash
# create virtual environment
python -m venv .venv

# activate virtual environment
# on Windows:
.venv\Scripts\activate
# on macOS/Linux:
source .venv/bin/activate

# install dependencies
pip install -r requirements.txt

# set API key for LLM access (replace with actual key)
# on Windows:
$env:GROQ_API_KEY = "gsk_..."
# on macOS/Linux:
export GROQ_API_KEY="gsk_..."

# start application
uvicorn server:app
```

## Test

<p align="center">
  <img width="686" height="913" alt="Bildschirmfoto 2026-03-30 um 14 53 50" src="https://github.com/user-attachments/assets/93adae6f-c38b-4a11-9c15-e2e5ea3b25cd" />
</p>

```bash
Hi, my name is John Smith (friends call me Johnny).  
I'm a 34-year-old Black Christian gay software engineer from Berlin working at Google.  
My blind wife Mary Johnson studies at Harvard University.  
You can reach me at john.smith@example.com or call me on +4312345678.  
We'll meet the European Council delegation on 12 July 2025 at 3:00 pm.
```
