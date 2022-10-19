FROM python:3.8-slim-buster

COPY requirements.txt .
COPY ./ ./producer

RUN pip install --upgrade pip && pip install -r requirements.txt && python -m spacy download en_core_web_sm

ENTRYPOINT ["tail", "-f", "/dev/null"]