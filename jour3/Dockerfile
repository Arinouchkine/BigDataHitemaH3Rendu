FROM ubuntu
RUN mkdir work
WORKDIR ./work
RUN apt-get update
RUN apt-get -y  install python3.6
RUN apt-get -y install python3-pip
RUN pip3 install jupyter
RUN pip3 install pandas
RUN pip3 install numpy
RUN pip3 install seaborn
RUN apt-get -y install git
# RUN git config --global user.email johndoe@example.com
# RUN  git config user.password "your_psw"
# RUN git pull url_git
EXPOSE 8889
CMD ["sh","-c","jupyter notebook --ip 0.0.0.0 --port 8889 --allow-root"]

