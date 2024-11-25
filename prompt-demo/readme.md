docker build -t bhavyabapna/docker-prompt . --push

docker run -it bhavyabapna/docker-prompt

The -it flag ensures that the container runs interactively, allowing you to provide input when the script prompts for it.
