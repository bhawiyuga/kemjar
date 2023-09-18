# Use the official Kali Linux image as the base image
FROM kalilinux/kali-rolling

# Update the package list and install the required tools
RUN apt-get update && \
    apt-get install -y nmap iputils-ping tshark dsniff python3-pip && \
    rm -rf /var/lib/apt/lists/*

RUN pip3 install scapy

# Set the default command to start an interactive shell
CMD ["bash"]