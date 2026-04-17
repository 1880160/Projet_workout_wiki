# Projet Workout's Wiki
## Testing: 
```bash
#Create env
python -m venv python-env
#Update envenronnment
pip install -r ./requirements

#start serving a static page:
mkdocs serve
```
## Using auto translation from en to any language
1. create a .env file in the docs folder
2. put your lingo.dev api key inside
3. run ``` npx lingo.dev@latest run ```
