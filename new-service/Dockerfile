# Use the official Ubuntu base image
FROM ubuntu:latest

# Run apt-get update
RUN apt-get update && apt-get install -y sudo

# Create a user named myuser and set up a basic environment
RUN useradd -m -s /bin/bash myuser

# Set the default user for the container
USER myuser

# Connect to the new user's home directory
WORKDIR /home/myuser

# Keep the container running in the background so it stays active in Docker Desktop
CMD ["sleep", "infinity"]
