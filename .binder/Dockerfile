FROM rocker/binder:4.4.0
LABEL maintainer='Tra Bi Nene'
COPY --chown=${NB_USER} . ${HOME}
USER ${NB_USER}



RUN wget https://github.com/FranckTbn/holepunch-test/raw/master/DESCRIPTION && R -e "options(repos = list(CRAN = 'http://mran.revolutionanalytics.com/snapshot/2024-06-11/')); devtools::install_deps()"

RUN rm DESCRIPTION.1; exit 0
