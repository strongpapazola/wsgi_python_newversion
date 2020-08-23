# wsgi_python_newversion
WSGI with python3 newest version

<pre>
apt install software-properties-common 
add-apt-repository ppa:deadsnakes/ppa
apt update
apt install python3.7
apt install apache2 apache2-dev libapache2-mod-wsgi-py3
update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.7 1
update-alternatives --config python3
python3 -m pip install mod_wsgi
a2dismod wsgi
echo 'LoadModule wsgi_module "/usr/local/lib/python3.7/dist-packages/mod_wsgi/server/mod_wsgi-py37.cpython-37m-x86_64-linux-gnu.so"' >> /etc/apache2/apache2.conf
service apache2 restart
</pre>
