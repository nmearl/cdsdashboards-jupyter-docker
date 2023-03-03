ARG BASE_REPO=ideonate/jh-voila-oauth-singleuser
FROM $BASE_REPO

USER root

RUN apt update && apt install -y tk-dev && rm -rf /var/lib/apt/lists/*

USER $NB_UID

RUN pip install streamlit

RUN pip install dash 'plotlydash-tornado-cmd>=0.0.6'

RUN pip install bokeh panel 'bokeh-root-cmd>=0.0.5'

RUN pip install git+https://github.com/cosmicds/hubbleds.git

RUN pip install importlib_metadata --upgrade

# Leave user as jovyan to avoid accidental container runs as root
