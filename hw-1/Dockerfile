FROM python:3

ARG IS_READY

WORKDIR /app

VOLUME /app/content

COPY main.py main.py

RUN if [ "$IS_READY" = "true" ] ; then echo "We are ready" > index.html; else echo "We are not ready" > index.html ; fi

CMD [ "python3", "main.py" ]

EXPOSE 8080
