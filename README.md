# Catetan Linux

# Sistem
## Mengatur proxy

###### export proxy dengan ketik di terminal
	export http_proxy=http://ITS-547987-25879:66c4f@proxy.its.ac.id:8080
	export https_proxy=http://ITS-547987-25879:66c4f@proxy.its.ac.id:8080

###### lalu edit __/etc/apt/apt.conf__ :
	Acquire::http::proxy "http://proxy.company.com:80/";
	Acquire::https::proxy "https://proxy.company.com:80/";
	Acquire::ftp::proxy "ftp://proxy.company.com:80/";

## Restart service

###### ketik di terminal :
	sudo service nama_service restart


# GITHUB

###### push github tanpa login selama 2 jam
	git config --global credential.helper 'cache --timeout 7200'
