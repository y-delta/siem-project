# Using Alpine Linux as base image
FROM Alpine:latest

# Install Suricata
RUN apk add --no-cache Suricata

# Copy Suricata configuration file
COPY suricata.yml /etc/suricata/suricata.yml

# Define default run command
CMD ["suricata", "-c", "/etc/suricata/suricata.yml", "-i", "eth0"]