# Assets in the rotki database

`rotki` ([rotki.com](https://rotki.com)) is a portfolio management, analytics and accounting application that protects your privacy. It is a local app, the code is open source and available at [github](https://github.com/rotki/rotki).

At rotki, each instance keeps a database that can be found [here](https://github.com/rotki/rotki/blob/develop/rotkehlchen/data/global.db) called `global.db`. It contains information about contracts and assets that can be used by the user when the app is used for the first time. If the app detects that the DB is missing we copy the packaged one so the user has acccess to all this information from the start. We update it periodically with more assets and also the user can add/edit/delete assets and other information from its local copy.

As part of the Advent of crypto Data we are releasing CSV files from this database compiled with all data up to version 1.31.1 of the rotki app to be easily used by others in their apps along with a script to generate them from any version after the one mentioned.

You can read the [jupyter notebook](rotki_assets.ipynb) where we do an analysis of the data and provide more information.