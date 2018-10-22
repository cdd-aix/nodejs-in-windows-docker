FROM microsoft/windowsservercore:ltsc2016
ENV chocolateyUseWindowsCompression false
SHELL ["powershell", "-Command", "$errorActionPreferences = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]
# RUN iex ((new-object net.webclient).DownloadString('https://chocolatey.org/install.ps1'))
RUN choco --help
# RUN choco install -y nodejs-lts --version 8.12.0
RUN npm install --global --production hello-world-npm; hellow-world-npm
# RUN npm install --global --production bcrypt@^3.0.2
