
## Setup

```bash
pip install google-adk
```

```bash
gcloud init
gcloud init --skip-diagnostics
gcloud auth login
gcloud auth application-default login
```

```bash
export GOOGLE_CLOUD_PROJECT=`gcloud config list --format 'value(core.project)'`
export GOOGLE_CLOUD_LOCATION=us-central1
```

```bash
echo "GOOGLE_GENAI_USE_VERTEXAI=TRUE" > ./multi_tool_agent/.env
echo "GOOGLE_CLOUD_LOCATION=us-central1" >> ./multi_tool_agent/.env
echo "GOOGLE_CLOUD_PROJECT=$GOOGLE_CLOUD_PROJECT" >> ./multi_tool_agent/.env
```

## Run

```bash
adk web
```
