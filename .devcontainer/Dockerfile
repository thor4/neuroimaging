FROM continuumio/anaconda3

COPY requirements.txt /tmp/pip-tmp/

RUN apt-get update && conda update -n base -c defaults -y conda && conda install -y --channel conda-forge nipype && pip install -r /tmp/pip-tmp/requirements.txt && rm -rf /tmp/pip-tmp