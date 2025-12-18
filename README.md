
# openwebui-docker-serverless

An experiment with Open WebUI and Docker to use Scaleway serverless infrastructure.

## Setup

Before running the project, copy the example environment file and fill in your secrets and configuration:

```sh
cp .env.local.example .env.local
# Then edit .env.local to add your actual secrets and configurations
```

## Usage

This sandbox/example uses Docker Compose and npm scripts for convenience.

Make sure you have your Docker Engine/runtime/daemon running.

### Scripts

- **Start normally:**
	```sh
	npm start
	```

- **Start fresh (stateless, mimics serverless cold start):**
	```sh
	npm run start:fresh
	```

- **Stop containers:**
	```sh
	npm stop
	```

- **Clean up everything (remove containers, volumes, orphans):**
	```sh
	npm run clean
	```

- **Full clean restart:**
	```sh
	npm run restart
	```

Open http://localhost:8080 on your browser.