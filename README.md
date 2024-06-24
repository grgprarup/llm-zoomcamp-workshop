# llm-zoomcamp-workshop

## Install Pipenv
```
pip install pipenv
```

## Install packages
```
pipenv install tqdm notebook==7.1.2 openai elasticsearch
```

## OpenAI API Key
Create .envrc file and add the following line
Get key from
https://platform.openai.com/api-keys
```
export OPENAI_API_KEY="Token"
```

## Start Jupyter Notebook
```
pipenv run jupyter notebook
```

## Install direnv
```
sudo apt update
sudo apt install direnv 
direnv hook zsh >> ~/.zshrc  (direnv hook bash >> ~/.bashrc)
```

## Export key
```
direnv allow
```

## Run elasticsearch in docker
```
docker run -it --name elasticsearch -p 9200:9200 -p 9300:9300 -e "discovery.type=single-node" -e "xpack.security.enabled=false" docker.elastic.co/elasticsearch/elasticsearch:8.4.3
```

## Verify elasticsearch
```
curl localhost:9200
```




