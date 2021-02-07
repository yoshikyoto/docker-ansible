FROM python:3.8-buster

# ssh サーバーをインストールして、
# sshd を起動刷るのに必要な sshd ディレクトリを作成
RUN apt-get update -y \
 && apt-get install -y openssh-server \
 && mkdir /var/run/sshd
EXPOSE 22

CMD ["/usr/sbin/sshd", "-D"]
