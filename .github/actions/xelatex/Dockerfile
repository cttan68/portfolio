#FROM ubuntu:latest
FROM texlive/texlive:latest

MAINTAINER Chin Thong <chinthongtan68@gmail.com>
# LABEL "maintainer"="Chin Thong <chinthongtan68@gmail.com>"
LABEL   "repository"="https://github.com/cttan68/portfolio" "homepage"="https://github.com/cttan68/portfolio"
LABEL   "com.github.actions.name"="Convert to PDF" "com.github.actions.description"="Convert documents to PDF using pdflatex." "com.github.actions.icon"="code" "com.github.actions.color"="blue"
#ENV TZ=Asia/Singapore
#RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

# Install all xelatex and LaTeX dependencies
#RUN apt-get update && \
#    apt-get install --yes --no-install-recommends \
#    texlive-fonts-extra \
#    texlive-fonts-recommended \
#    texlive-latex-recommended \
#    texlive-lang-english \
#    texlive-xetex && \
#    apt-get autoclean && apt-get --purge --yes autoremove && \
#    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
ADD entrypoint.sh /entrypoint.sh
RUN chmod +x /entrypoint.sh
ENTRYPOINT ["/entrypoint.sh"]
