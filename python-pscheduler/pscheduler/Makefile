#
# Makefile for python-pscheduler module
#

default: build


test:
	nosetests

test-coverage:
	nosetests --with-coverage --cover-package rabbitmq


build: test
	python setup.py build

clean:
	make -C tests $@
	find . -name "*.pyc" | xargs rm -f
