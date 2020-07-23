First of all, you need to have Docker installed in your machine.<br />
[Get Docker installed](https://docs.docker.com/get-docker/)<br/><br/>

In the example directory, you can run:

### `sudo docker image build -t ex-build-dev .`

Sends build context to Docker daemon.

### `sudo docker container run -it -v $(pwd):/app -p 80:8000 --name python-server ex-build-dev`

Runs the container.
You can also open [http://localhost:80](http://localhost:80) to view it in the browser.
