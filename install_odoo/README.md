# Installer Odoo 15 sur une machine locale
```
sudo apt update 
sudo apt upgrade 
sudo apt install python3-dev python3-pip python3-wheel python3-venv
sudo apt install build-essential libpq-dev libxslt-dev libzip-dev libldap2-dev libsasl2-dev libssl-dev


sudo apt-get install postgresql
sudo su - postgres
createuser --createdb --no-createrole --superuser --pwprompt odoo14
psql
\du


sudo apt-get install git
git clone https://www.github.com/odoo/odoo --depth 1 --branch 15.0 --single-branch .


venv
python3 -m venv ~/odoo/15.0/.env
source ~/odoo/15.0/.env/bin/activate
pip3 install setuptools wheel
pip3 install -r requirements.txt


python3 ce/odoo-bin -r odoo14 -w odoo14 --db_host localhost --db_port 5432



sudo wget https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.bionic_amd64.deb
sudo dpkg -i wkhtmltox_0.12.5-1.bionic_amd64.deb
sudo apt install -f
```