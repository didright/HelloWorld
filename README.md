version: '3'
services:
  jupyter-tutorial:
    image: jupyter/base-notebook
    container_name: jupyter-notebook
    ports:
      - "1688:1688"
    volumes:
      - ./work:/home/jovyan/work/
    command: start-notebook.sh --NotebookApp.token=''
