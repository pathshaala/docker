FROM ubuntu:jammy

RUN apt update && apt install -y cowsay

COPY deep.cow /usr/share/cowsay/cows/
# COPY babyyoda.cow /usr/share/cowsay/cows/

ENV PATH $PATH:/usr/games


## First: if user want to give custom msg then s/he has to provide full cmd eg: docker run deepsay cowsay -f ddep.cow custom msg
# CMD ["cowsay","-f","deep.cow","Hello"]

## Second; hardcoded hello whatever user will provide it wil append with it.
# ENTRYPOINT ["cowsay","-f","deep.cow","Hello"]

## Third; user always has to provide input not default value
# ENTRYPOINT ["cowsay","-f","deep.cow"]

## Final: deafult value is hello and if user will privide any custom msg 
CMD ["Hello"]
ENTRYPOINT ["cowsay","-f","deep.cow"]