.PHONY: build_python build_pyspark build_scala

build_python:
	docker build -t python-app ./python

build_pyspark:
	docker build -t pyspark-app ./pyspark

build_scala:
	docker build -t scala-app ./scala

run_python:
	docker run --rm python-app python hello_world.py

run_pyspark:
	docker run pyspark-app

run_scala:
	docker run --rm scala-app scala HelloWorld

build: build_python build_pyspark build_scala

run: run_python run_pyspark run_scala
