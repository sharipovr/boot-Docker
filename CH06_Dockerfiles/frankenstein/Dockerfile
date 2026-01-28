FROM python:3
COPY main.py main.py
COPY books/ books/
RUN apt update && apt install -y python3
CMD ["python", "main.py"]