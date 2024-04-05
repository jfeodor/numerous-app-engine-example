FROM mcr.microsoft.com/devcontainers/python:3.11

RUN apt update && apt install -y dbus dbus-user-session gnome-keyring

# enable keyring
COPY .bashrc.keyring /home/vscode/.bashrc.keyring
RUN echo ". ~/.bashrc.keyring" >> /home/vscode/.bashrc

RUN pip install numerous[dev]>=0.33
RUN pip install marimo streamlit dash
