# Serverless Prisma

[![Build Status](https://travis-ci.org/jgeschwendt/serverless-prisma.svg?branch=master)](https://travis-ci.org/jgeschwendt/serverless-prisma)

**[Archived]** — New projects should consider using [Prisma2](https://www.prisma.io/blog/announcing-prisma-2-zq1s745db8i5#getting-started-with-prisma-2)

Minimal Serverless + Prisma Project Template

## Getting Started

- Be sure to have `Docker` and `Make` installed on your machine. `Docker` is used for maintaining a consistent development/deployment environment; `Make` is used to shorten frequently used `Docker` commands.

- Create an `.env` file for your local machine (refer to `~/.env.example` for the configuration requirements)

- Create Environment configurations for deployments, ie. `.env.dev`, `.env.prod`, alternatively this can be configured in your CI/CD.

```console

# Create a Node Development Docker Container

make devbox


# Install Node Dependencies using the DevBox Container

make install


# Start Serverless in Offline Mode

make start


# Package Service for Deployment

make build


# Deploy to a specific Environment

ENV=dev make deploy                     # uses the configuration from `.env.dev`

ENV=prod make deploy                    # uses the configuration from `.env.prod`

```

The complete command list can be viewed in the `~/Makefile`
