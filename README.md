# All in AI Demo App

<div align="center">
  <a href="https://dash.plotly.com/project-maintenance">
    <img src="https://dash.plotly.com/assets/images/maintained-by-plotly.png" width="400px" alt="Maintained by Plotly">
  </a>
</div>

A demo app for the [All in AI](https://allinevent.ai/) presentation on September 27, 2023.

Developed & presented by Nathan Drezner ([@ndrezn](https://github.com/ndrezn)).


https://github.com/plotly/all-in-ai-demo-app/assets/32049495/35f40db8-e83d-4ad7-af9b-a9390f696bde


This application uses [Dash Chart Editor](https://github.com/BSd3v/dash-chart-editor) and the [OpenAI Python library](https://github.com/openai/openai-python) to build an application allowing users to ask questions about a dataset and persist views of their dataset with analytics associated.

Once a dataset is uploaded, context on that dataset is added to the prompt for the chat window, and users can interact with the dataset with natural language. After building charts, users can click the "Copy link" button to save those charts to a permanent link, using Redis to save state.

<p align="center">
    <img src="screenshots/4.png", width=500>
</p>


## Usage
> Note: You must provide an [OpenAI API key](https://platform.openai.com/account/api-keys) as an environment variable at `$OPEN_AI_KEY`.

Install the dependencies with:
```
pip install -r requirements.txt
```

And run the application with:
```
python app.py
```

Or, provide your API key directly if it is not in your environment:
```
OPEN_AI_KEY=... python app.py
```


annotated-types==0.7.0
anyio==4.4.0
async-timeout==4.0.3
blinker==1.8.2
certifi==2024.7.4
charset-normalizer==3.3.2
click==8.1.7
dash==2.17.1
dash-bootstrap-components==1.6.0
dash-chart-editor==0.0.1a5
dash-core-components==2.0.0
dash-html-components==2.0.0
dash-mantine-components==0.13.0a2
dash-table==5.0.0
dash_ag_grid==31.2.0
distro==1.9.0
exceptiongroup==1.2.1
filelock==3.15.4
Flask==3.0.3
fsspec==2024.6.1
gunicorn==22.0.0
h11==0.14.0
httpcore==1.0.5
httpx==0.27.0
huggingface-hub==0.23.4
idna==3.7
importlib_metadata==8.0.0
itsdangerous==2.2.0
Jinja2==3.1.4
MarkupSafe==2.1.5
mpmath==1.3.0
nest-asyncio==1.6.0
networkx==3.1
numpy==1.24.4
openai==1.35.10
packaging==24.1
pandas==2.0.3
pillow==10.4.0
plotly==5.22.0
pydantic==2.8.2
pydantic_core==2.20.1
python-dateutil==2.9.0.post0
pytz==2024.1
PyYAML==6.0.1
redis==5.0.7
regex==2024.5.15
requests==2.32.3
retrying==1.3.4
safetensors==0.4.3
six==1.16.0
sniffio==1.3.1
sympy==1.13.0
tenacity==8.5.0
tokenizers==0.19.1
torch==2.2.2
torchvision==0.17.2
tqdm==4.66.4
transformers==4.42.3
typing_extensions==4.12.2
tzdata==2024.1
urllib3==2.2.2
Werkzeug==3.0.3
zipp==3.19.2