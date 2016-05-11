FROM caffe:cpu

RUN pip install jupyter

RUN mkdir -p /root/.jupyter/ && \
    echo "c.NotebookApp.ip = '*'" > /root/.jupyter/jupyter_notebook_config.py && \
    echo "c.NotebookApp.port = 8888" >> /root/.jupyter/jupyter_notebook_config.py && \
    echo "c.NotebookApp.open_browser = False" >> /root/.jupyter/jupyter_notebook_config.py

EXPOSE 8888
