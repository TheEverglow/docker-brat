# Dockerizing brat 
https://brat.nlplab.org

1) First, build an image: 
    ```sh
    $ docker build --build-arg user_name=USERNAME --build-arg password=PASSWORD --build-arg admin_email=EMAIL -t brat-app
    ```

2) To start it use the following command:
    ```sh 
    $ docker run -p 8001:8001 brat-app
    ``` 
    (use flag ```-d``` additionaly to run it in background)

3) Use website 127.0.0.1:<used port> from console (if you run in foreground) or print it manually in any browser
