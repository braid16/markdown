# step to deploy rails in ubunut 18.04
sudo apt update && upgrade
sudo apt install git curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev software-properties-common libffi-dev nodejs yarn
cd
wget http://ftp.ruby-lang.org/pub/ruby/2.5/ruby-2.5.3.tar.gz
tar -xzvf ruby-2.5.3.tar.gz
cd ruby-2.5.3/
./configure
make
sudo make install
ruby -v
gem install bundler
sudo apt-get install -y dirmngr gnupg
sudo service nginx start
