FROM httpd:latest
COPY . .

RUN apt-get update && apt-get install -y python

ARG user_name
ARG password
ARG admin_email

RUN sh install.sh $user_name $password $admin_email

CMD ["python", "standalone.py"]



