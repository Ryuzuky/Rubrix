# Rubrix #
Weak Supervision with Rubrix

## Installation ## 

- Open terminal (e.g. Powershell), use `cd` to move to the desired directory, then clone this repository into local machine  
`git clone "https://github.com/Ryuzuky/Rubrix.git"`  

- Install docker  
`https://docs.docker.com/engine/install/`

 - Launch the web app  
`docker run -d --name elasticsearch-for-rubrix -p 9200:9200 -p 9300:9300 -e "ES_JAVA_OPTS=-Xms512m -Xmx512m" -e "discovery.type=single-node" docker.elastic.co/elasticsearch/elasticsearch-oss:7.10.2`  

- Install all dependencies in requirements.txt  
`pip install -r requirements.txt`  

- Running the App at localhost:6900  
`python -m rubrix`
