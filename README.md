# deck-wp - A Docker Deck for WordPress Installation.

A Docker Deck is a Docker Compose file or files that make creating a docker container just a bit easier.

Docker Decks try to adhere to the following:
* most configuration is done using the .env file, avoiding unneccesarily editing the docker-compose.yml file
* defaults to using persistent volumes

Deck-wp can be used to easily create a docker container that runs the Docker WordPress image.

### Prerequisites

* Docker is installed locally or within a Virtual Machine (e.g: Virtual Box)
* you are logged into the host and are either root or are a member of the Docker group
* docker-compose is installed

### Quick Start


    curl -L https://github.com/ajdruff/deck-wp/archive/master.tar.gz | tar -zx
    mv deck-wp* example.com
    cd example.com
    mv .env-sample .env
    docker-compose up




### Detailed Installation Steps

download manually

Go to https://github.com/ajdruff/mod-wp and click 'Clone or Download' and click the 'Download ZIP' link, or download from https://github.com/ajdruff/mod-wp/archive/master.zip

Extract mod-wp-master.zip to your site's root folder (e.g: public_html or htdocs)

Rename the parent directory from mod-wp-master to mod-wp
download using git clone

    cd /path/to/webroot/
    git clone https://github.com/ajdruff/mod-wp.git
download using wget

     cd /path/to/webroot/ 
     wget -qO- https://github.com/ajdruff/mod-wp/archive/master.tar.gz | tar -zx
     mv mod-wp* mod-wp
download using curl

    cd /path/to/webroot/
    curl -L https://github.com/ajdruff/mod-wp/archive/master.tar.gz | tar -zx
    mv mod-wp* mod-wp
Your website's directory structure should now look something like this :

                public_html
                    ├───mod-wp

#Configuration

Configuration of the container should be done primarily using the `.env` file.





#Creating the Container



## Contributing

1. Fork it!
2. Create your feature branch: git checkout -b my-new-feature
3. Commit your changes: git commit -am 'Add some feature'
4. Push to the branch: git push origin my-new-feature
5. Submit a pull request :D




## Authors

* **Andrew Druffner** andrew@nomstock.com

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

