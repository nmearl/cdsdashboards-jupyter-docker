ARG BASE_REPO=ideonate/jh-voila-oauth-singleuser
FROM $BASE_REPO

USER $NB_UID

# RUN pip install streamlit

# RUN pip install dash 'plotlydash-tornado-cmd>=0.0.6'

# RUN pip install bokeh panel 'bokeh-root-cmd>=0.0.5'

RUN pip install git+https://github.com/Carifio24/hubbleds.git@no-data

RUN pip install importlib_metadata --upgrade

RUN sudo apt-get install tk-dev

# Leave user as jovyan to avoid accidental container runs as root
