FROM nodered/node-red:latest
USER root

# Install Python
RUN apk add python3 py3-pip
RUN pip install pynmea
RUN pip install pyais

WORKDIR /usr/src/node-red
USER node-red

# Install the dashboard extension
RUN npm install node-red-dashboard

# Install Azure IoT Edge Module nodes
RUN npm install node-red-contrib-azure-iot-edge-module
