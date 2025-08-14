## Setup

#### Step 1 - Installation & Initialisation

- Clone the repo and run `git submodule update --init` at the root.
- Run `pnpm i` at the root

#### Step 2 - Build and Run locally

- Goto Github > Settings > Developer Settings > OAuth Apps > Create a new app for citypulse

1. Homepage URL : https://citypulse-web.citypulse.localhost
2. Callback URL : https://citypulse-service.citypulse.localhost/github/callback

- Export the GITHUB_CLIENT_ID and GITHUB_CLIENT_SECRET in the terminal

- Then, run `docker compose up --build` at the root.

#### Step 3 - Open Apps in the browser

The certificates are local self signed certificates which causes the browser to show warning screen. So, we will need to 

1. https://citypulse-service.citypulse.localhost/ - first open this in browser and trust the link

2. https://citypulse-web.citypulse.localhost/ - similarly open this in browser and trust the link

You should be able to access the apps running locally.
