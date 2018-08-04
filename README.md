# Important-Dockerfiles
A list of import basic dockerfiles 

Building Image : <br>
```docker build --network=host -t image_name -f dockerfile_name .```
<br><br>
Creating container from Image: <br>
```nvidia-docker run -itd -v local_dir:container_dir --net=host image_name bash```
<br><br>
Going inside a container:<br>
```docker exec -it container_id bash```


*Use nvidia-docker when you are building container in GPU, otherwise use docker*

Starting JupyterLab server:<br>
```jupyter lab --no-browser --ip 0.0.0.0 --port 9999 --allow-root```
