# Use the official Node 20 LTS image as a base
FROM node:20

# Ensure apt is up to date and install git (so WebStorm's Git support works)
RUN apt-get update \
    && apt-get install -y --no-install-recommends \
       git \
       bash \
    && rm -rf /var/lib/apt/lists/*

# Expose a commonly-used port (e.g. for running "npm start" or tests)
EXPOSE 3000

# When the container starts, drop into a shell by default.
CMD ["bash"]
