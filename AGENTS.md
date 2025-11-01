# openwebui-docker-sandbox

This repository is an experiment with Open WebUI and Docker to use Scaleway serverless infrastructure.

At the moment I am trying to create a sample/example Dockerfile to run Open WebUI with a remote database (through environment variables) that is hosted on Scaleway serverless DB service. My idea is to test this sample Dockerfile locally and then try to move it to Scaleway managed container service and possibly have a serverless service to run Open WebUI.

Open WebUI will also need information about the models, and I also expect to use a serverless inference service (with an OpenAI compatible API) from Nscale.