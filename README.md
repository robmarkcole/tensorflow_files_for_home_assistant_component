# tensorflow_files_for_github
All the files you need for the Home-Assistant [tensorflow component](https://www.home-assistant.io/components/image_processing.tensorflow/).

Just `git clone` this repo, then copy the `tensorflow` folder into your configuration directory.

FYI utils has the function that maps the integers returned by the model to the actual category, data has the actual mappings, and proto is how tensorflow object detection tensor gets the data.

## Hassbian advice
To install tensorflow, you need to have permissions of the `homeassistant` user and activate the python venv that HA uses.
* Set user -> `sudo -u homeassistant -H -s`
* Activate venv -> `cd /srv/homeassistant/` then `source bin/activate`
* `pip3 install tensorflow==1.13.2`
