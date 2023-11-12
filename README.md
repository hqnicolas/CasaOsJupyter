# CasaOsJupyter
Runing Jupyter Notebook on CasaOS Server with aarch64

- to change your docker external port:
```
published: "3001"
```
to access the login token:
1. On Casaos Home
2. Click on Jupyter3 Config
3. Click on Terminal and Logs
4. on Logs, Find this line:
```
jupyter3-jupyter3-1  | [I 08:47:36.603 NotebookApp] http://4cf6b5299e86:8888/?token=70debeb437bbd2587
```
Take the Link 

- This file is Based on Comand:
```
docker run -i -t -p 3001:8888 -v "$PWD":/workspace --name jupyter3 konmeo/jupyter /bin/bash -c "\
jupyter notebook \
--notebook-dir=/workspace --ip='*' --port=8888 \
--no-browser --allow-root"
``` 
