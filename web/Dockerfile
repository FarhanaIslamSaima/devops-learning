FROM python:3.11-slim
COPY . /app
WORKDIR /app

RUN python3 -m venv /opt/venv

RUN pip install --upgrade pip && \
    /opt/venv/bin/pip install -r requirements.txt && \
    chmod +x entrypoint.sh


CMD ["/app/entrypoint.sh"]