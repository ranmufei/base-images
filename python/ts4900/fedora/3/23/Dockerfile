FROM resin/ts4900-fedora-buildpack-deps:23

# http://bugs.python.org/issue19846
# > At the moment, setting "LANG=C" on a Linux system *fundamentally breaks Python 3*, and that's not OK.
ENV LANG C.UTF-8

RUN dnf install -y \
		python3-pip \
		python3-dbus \
	&& dnf clean all

# install "virtualenv", since the vast majority of users of this image will want it
RUN pip3 install -U --no-cache-dir --ignore-installed pip setuptools \
	&& pip3 install --no-cache-dir virtualenv

CMD ["echo","'No CMD command was set in Dockerfile! Details about CMD command could be found in Dockerfile Guide section in our Docs. Here's the link: http://docs.resin.io/deployment/dockerfile"]
