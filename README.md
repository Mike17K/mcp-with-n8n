# mcp-with-n8n
the simplest way to custom create an ai agent, you will need the following
1. docker desktop installed and running
download the installer [here](https://docs.docker.com/desktop/setup/install/windows-install/).
3. thats it!

# Steps
1. Run the command bellow to run the n8n image with options:
to run on start
to expose standard port
to keep files persistant on machine
enable the community packages as tools
```bash
docker volume create n8n_data

docker run --restart always --name n8n -e N8N_COMMUNITY_PACKAGES_ALLOW_TOOL_USAGE=true -p 5678:5678 -d -v n8n_data:/home/node/.n8n docker.n8n.io/n8nio/n8n
```

2. install the n8n-nodes-mcp from within ui

the image if interested for latest versions is: https://hub.docker.com/r/n8nio/n8n

Give me a star if liked it!
Have fun!
