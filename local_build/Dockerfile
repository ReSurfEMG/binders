FROM python:3.9

ENV PYTHONUNBUFFERED 1
WORKDIR /usr/src/app

RUN apt update && apt-get install libsasl2-dev python3-dev libldap2-dev libssl-dev -y
COPY requirements.txt ./
RUN pip install -r requirements.txt

COPY . .

EXPOSE 8888
# CMD ["jupyter", "nbextension", "enable'", "--py", "widgetsnbextension"]
CMD ["jupyter", "notebook", "--ip='0.0.0.0'", "--port=8888", "--no-browser", "--allow-root"]