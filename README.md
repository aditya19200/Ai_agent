#ABOUT
.google adk is a framework to build Ai agents



##  Installation

You can install the ADK using `pip`:

```bash
pip install google-adk
```

##  Getting Started

Create your first agent (`my_agent/agent.py`):

```python
# my_agent/agent.py
from google.adk.agents import Agent
from google.adk.tools import google_search

root_agent = Agent(
    name="search_assistant",
    model="gemini-2.0-flash-exp", # Or your preferred Gemini model
    instruction="You are a helpful assistant. Answer user questions using Google Search when needed.",
    description="An assistant that can search the web.",
    tools=[google_search]
)
```

Create `my_agent/__init__.py`:

```python
# my_agent/__init__.py
from . import agent
```

Run it via the CLI (from the directory *containing* `my_agent`):

```bash
adk run my_agent
```

Or launch the Web UI from the folder that contains `my_agent` folder:

```bash
adk web
```

#screenshot
![WhatsApp Image 2025-04-11 at 20 28 03_8a693072](https://github.com/user-attachments/assets/b27962b3-7f0b-4b25-ae78-df24b0b53f13)


