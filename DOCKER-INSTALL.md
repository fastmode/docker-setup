# Deploy EAACI Horizontal Interactive Panel
## Requirements
1. Windows 10 Pro computer
2. Set Display settings to 1920 x 1080
3. Google Chrome

## Install Docker and run App
1. Navigate to [Docker Hub](https://hub.docker.com/editions/community/docker-ce-desktop-windows)
2. Create free account to download Docker Desktop (541MB)
3. Ensure Docker Desktop is installed with administrative user.  Install with Default options.
4. Ensure to enable Hyper-V virtualization when prompted toward the end of the installation.  Computer will restart.
5. Upon restart, check task bar and allow Docker Desktop to complete loading.   Open Command Prompt as an Admin.
6. Run command: `docker version` to ensure docker was installed successfully.
7. Run command:  `docker run -p 80:80 <username>/<image-name>` to download and start the application.  
8. Click "Allow access" if you get a Windows Security Alert prompt.
9. Depending on internet speed, download and build should around 3 minutes.
10. Open Chrome and navigate to: `localhost`   The application will load if the build is completed.
11. Click on the Chrome menu and make toggle Fullscreen.


## To stop the app
1. To stop the application, in the Command Prompt window, press Ctrl-C or Ctrl-X
2. Type `docker ps -a` to see running containers.  Copy the Container ID of the running instance.
3. Type `docker stop <ContainerID>` to stop the container from running.

## To start the app
1. Ensure the container is stopped, see "To stop the app"
2. Run command:  `docker run -p 80:80 <username>/<image-name>` to start the application.
