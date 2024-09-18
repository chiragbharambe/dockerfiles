# Dockerfiles
My various dockerfiles

# ComphyUI
To use this Dockerfile:

1. Save the Dockerfile in your project directory.
2. Build the Docker image:
   ```
   docker build -t comfyui .
   ```
3. Run the container:
   ```
   docker run -it --gpus all -p 8188:8188 -v /path/to/your/models:/app/models comfyui
   ```

Remember to replace `/path/to/your/models` with the actual path to your models directory on your host machine.

This setup will create a Docker container with ComfyUI and all the specified dependencies installed, running on Alpine Linux with Python 3.11 and CUDA support.
