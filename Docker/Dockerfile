FROM ubuntu


RUN apt update
RUN touch deren.txt
RUN apt install python3 -y

ENV PORT 80

EXPOSE $PORT

CMD ["sh", "-c", "python3 -m http.server $PORT"]
