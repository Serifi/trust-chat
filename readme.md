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

**Input**
```bash
Hi, my name is John Smith (friends call me Johnny).  
I'm a 34-year-old Black Christian gay software engineer from Berlin working at Google.  
My blind wife Mary Johnson studies at Harvard University.  
You can reach me at john.smith@example.com or call me on +4312345678.  
We'll meet the European Council delegation on 12 July 2025 at 3:00 pm.
```

**Output**
```bash
User: Hi, my name is ID-a8294a56 (friends call me ID-a66f7b25).  
I'm a ID-0ae49774 [ID03] [ID02] [ID04] software engineer from ID-d6572886 working at ID-588107e2.  
My [ID05] [ID01] ID-5a07a57c studies at ID-64966eb7.  
You can reach me at ID-c7e1675f or call me on ID-2161481c.  
We'll meet ID-a04135f9 delegation on ID-bd7372ed at ID-cde511be.

TrustChat: Hi ID-7ac1c86b! Great to meet you. Thanks for introducing yourself, ID-e3682c01.
Working at ID-a92b20bc as a software engineer in ID-35b0e53c sounds like an exciting career.
Please send any further details to ID-6eadf1d2 or I can reach you at ID-b9f90147.
Regarding your upcoming meeting with ID-685974f1 on ID-52ea34b8 at ID-4f7cb30a, I hope it goes smoothly!
Also, please pass along my regards to ID-6eb0ebb1 at ID-41d6156d.
```
