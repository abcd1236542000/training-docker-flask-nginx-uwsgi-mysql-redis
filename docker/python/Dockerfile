# ベースイメージ
FROM python:3.7

RUN mkdir /var/www
# workdirの指定

# 依存Pythonライブラリ一覧コピー
COPY requirements.txt ./

RUN pip install --upgrade pip

# 依存Pythonライブラリインストール
RUN pip install -r requirements.txt

COPY uwsgi.ini /uwsgi.ini

CMD ["uwsgi", "--ini", "/uwsgi.ini"]
# CMD ["uwsgi","--ini","/var/www/uwsgi.ini"]
