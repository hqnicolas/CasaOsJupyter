# CasaOsJupyter
Runing Jupyter Notebook on CasaOS Server with aarch64
- Based on Comand:
-
' docker run -i -t -p 3001:8888 -v "$PWD":/workspace --name jupyter3 konmeo/jupyter /bin/bash -c "\
jupyter notebook \
--notebook-dir=/workspace --ip='*' --port=8888 \
--no-browser --allow-root" '
