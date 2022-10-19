FROM python:3.8-slim-buster

COPY requirements.txt .
COPY ./ ./consumer

RUN pip install --upgrade pip && pip install -r requirements.txt

ENTRYPOINT ["tail", "-f", "/dev/null"]