FROM smartislav/spark:2.3.0-jdk8u121

RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv E56151BF \
 && apt-get -y update \
 && apt-get -y install --no-install-recommends python-pip python-setuptools python-wheel \
 && apt-get clean -y \
 && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* \

RUN pip install PyYAML==3.12 \
 && pip install elasticsearch==5.4.0 \
 && pip install kafka==1.3.3 \
 && pip install python-dateutil==2.6.1
