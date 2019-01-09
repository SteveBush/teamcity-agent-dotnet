FROM jetbrains/teamcity-agent

RUN curl -s -O https://packages.microsoft.com/config/ubuntu/18.04/packages-microsoft-prod.deb && \
	apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 417A0893 && \
	add-apt-repository universe && \
	apt-get update && apt-get install -y --no-install-recommends apt-utils && \
	apt-get update && \
	dpkg -i packages-microsoft-prod.deb && \
	apt-get install apt-transport-https -y && \
	apt-get update && \
	apt-get install dotnet-sdk-2.2 -y
	