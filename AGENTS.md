# openwebui-docker-serverless

This repository is an experiment with Open WebUI and Docker to use Scaleway serverless infrastructure.

I have created a `docker-compose.yml` file and several helper scripts on `package.json` that allow me to mimic the serverless nature of Scaleway Serverless Containers service (when restarting the container all the volumes are dropped, etc).

The `docker-compose.yml` relies on `.env` files to set up the necessary ENV variables to make it work with stateless Scaleway Serverless Container service, and persist the necessary data on external services thus making the actual container truly serverless and transient.

I tested it on the Serverless Container service, by mimicking the config and environment variables and it works as expected.

I also used the serverless inference service (with an OpenAI compatible API) from Nscale, which also worked as expected.