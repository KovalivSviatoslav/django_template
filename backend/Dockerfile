FROM python:3

WORKDIR /usr/src/backend

COPY entrypoint.sh .
COPY ../poetry.lock .
COPY ../pyproject.toml .

RUN pip3 install poetry
RUN poetry config virtualenvs.create false
RUN poetry install --no-dev
RUN chmod +x entrypoint.sh

COPY . .

ENTRYPOINT ["/usr/src/app/entrypoint.sh"]