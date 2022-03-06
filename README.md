# Fastify + Svelte

Experimental frontend using [SvelteKit](https://kit.svelte.dev/).
The frontend calls the server api when a button is clicked, and renders the response.

### Install dependencies

```sh
npm install
```

### Run frontend dev server

```sh
# Configure backend URL to target from frontend dev server
# If this is unset, the same origin as the frontend dev server will be used.
export FULLSTACK_BACKEND=http://localhost:3001

npm run dev
```

### Build frontend
Builds static site into the `build` directory.

```sh
# Configure backend URL to target from statically compiled frontend
# If this is unset, the same origin as the static-build server will be used.
export FULLSTACK_BACKEND=https://yada.yada:xxxx

npm run build
```

### Developing with Gitpod
Cloning this repo and creating a Gitpod project will trigger automatic prebuilds 
when changes are committed to the repo.

The Gitpod workspace is configured to clone the backend repo into ../backend
and run `npm install` on both repos during prebuilds

Workspaces start with a backend server (running on port 3001) 
and a frontend dev server (running on port 3000).

