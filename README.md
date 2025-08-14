# codespaces-llm

This repository provides a GitHub Codespaces environment with [LLM](https://llm.datasette.io/), Python 3.13, `uv` and the GitHub Copilot VS Code extension.

**[Launch Codespace](https://codespaces.new/covolution/codespaces-llm?quickstart=1)**

Then try running this in a terminal:
```bash
llm "Fun facts about pelicans"
```
LLM is configured using the [llm-github-models](https://github.com/tonybaloney/llm-github-models) plugin for [llm](https://llm.datasette.io/en/stable/).

## Useful commands

```sh
llm models list - List the available models
llm "Tell me a joke about cats" -m github/gpt-4.1-mini
llm chat - start a chat session
```

## Templates
```
llm templates path
llm 'Summarize the following: ' --save summarize
llm -t summarize "A cat jumped over the mat"

llm 'Tell me a dad joke about $input' --save joke
llm -t joke "cats"
llm -t joke dogs
llm -t joke driving
llm templates
```

### Proof Read
To prove read some text : `llm -t read "I once went for a walk and it was grate but i ate chips"`

To prove read text in `input.txt` use `llm -t read < input.txt`