# Example usage 
```sh
sudo docker build --build-arg IS_READY="true" -t ready .
sudo docker run -p 8080:8080 -v hw-1/data:/app/content ready
curl localhost:8080/content/a.txt
```
