# kresus-docker-rpi

Reprise et modification du Dockerfile disponible sur kresusapp/app, afin de pallier à un problème.

L'entrypoint.sh d'origine installe la librarie lxml depuis pip (via requirements.txt)... Celà ne fonctionnant pas, et freeze l'install (???)
Le seul moyen (à ce stade) étant de débloquer l'install est d'installer python-lxml depuis apt-get

Ce repo rajoute donc la librairie depuis Dockerfile.
