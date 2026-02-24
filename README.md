# Prepare the OCI ununtu env.
1. Install Docker (Minimal)
bash
# Install Docker (convenience script for minimal setup)
curl -fsSL https://get.docker.com | sudo sh

# Add user to docker group (replace 'ubuntu' with your username if different)
sudo usermod -aG docker ubuntu

# Apply group changes without logout
newgrp docker

# Verify installation
docker --version

