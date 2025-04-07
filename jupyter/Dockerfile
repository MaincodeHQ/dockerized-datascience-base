FROM docker.io/jupyter/scipy-notebook:latest

USER root

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

RUN groupadd jovyan \
    && usermod -g jovyan -a -G users jovyan

USER jovyan

ENV NOTEBOOK_DIR=/home/jovyan/work/notebooks
ENV JUPYTERLAB_WORK_DIR=$NOTEBOOK_DIR

CMD ["start-notebook.sh", "--NotebookApp.notebook_dir=/home/jovyan/work/notebooks", "--allow-root", "--JupyterApp.token=''", "--JupyterApp.password=''", "--NotebookApp.use_lab=False"]