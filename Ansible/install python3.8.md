sudo yum update
sudo yum install gcc openssl-devel bzip2-devel libffi-devel
cd /opt
wget https://www.python.org/ftp/python/3.8.12/Python-3.8.12.tgz
tar xvf Python-3.8.12.tgz
cd Python-3.8.12
./configure --enable-optimizations
make -j 4
sudo make altinstall
python3.8 --version
echo 'export PATH="/usr/local/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
python3.8 -m venv /path/to/my/venv
source /path/to/my/venv/bin/activate
pip3.8 install requests
/usr/local/bin/python3.8 -m pip install --upgrade pip


sudo pip install virtualenv
virtualenv myenv
source myenv/bin/activate
pip3.8 install requests
deactivate

