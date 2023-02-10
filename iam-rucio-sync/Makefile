.ONESHELL:

BASETAG:=`cat BASETAG`

all: latest py2

latest:
	@docker build . -f Dockerfile --build-arg BASETAG=${BASETAG} --no-cache --tag iam-rucio-sync:latest
