FROM ubuntu:bionic
ENV JUPYTERLAB_VERSION 1.1.0
ENV USER_BINDER jovyan
ENV DEBIAN_FRONTEND noninteractive 
ENV DEB_BUILD_DEPS="sudo nano less git wget curl python3-dev python3-pip python3-setuptools"
ENV DEB_PACKAGES=""
ENV PIP_PACKAGES_COMMON="numpy"
ENV PIP_PACKAGES_KALE="kubeflow-kale==0.6.1"

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive && \
  echo "America/Mexico_City" > /etc/timezone && apt-get install -y tzdata

RUN apt-get update && apt-get install -y $DEB_BUILD_DEPS $DEB_PACKAGES && pip3 install --upgrade pip  

RUN curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash - && apt-get install -y nodejs            

RUN pip3 install jupyter "jupyterlab>=2.0.0,<3.0.0" --upgrade
 
RUN pip install --quiet "git+https://github.com/optimizacion-2-2021-1-gh-classroom/practica-1-segunda-parte-yefovar.git#egg=docs&subdirectory=src"

VOLUME ["/shared_volume"]

WORKDIR /

ENV NB_PREFIX opturl

ENTRYPOINT ["/usr/local/bin/jupyter", "lab", "--ip=0.0.0.0", "--no-browser", "--allow-root", "--LabApp.allow_origin='*'", "--LabApp.base_url=opturl"]
