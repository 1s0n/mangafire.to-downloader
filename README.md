# Mangafire Downloader

This is a ported version of [Mangareader.to Downloader](https://github.com/1s0n/Mangareader-Downloader-v2/)

# This does not work right now, but I have noticed that the images are not scrambled like mangareader.to, so I will now scrape the images instead of downloading them one by one like a user.

## How to run via terminal
To use this, ensure you have chromedriver_autoinstaller, selenium and PyMuPDF installed using pip, install them with command
```bash
pip3 install -r requirements.txt
```
Run ```main.py```, and enter the __link to the first page__ of the manga. eg. ```https://mangareader.to/read/kaguyasama-love-is-war-13/en/volume-1```

You can also pass it on as a argument. eg:
```bash
python3 main.py https://mangareader.to/read/kaguyasama-love-is-war-13/en/volume-1
```

## Batch downloader
To use the batch downloader, run batch.py, and enter the first volume/chapter of the manga you want to download
eg:
```
ENTER URL: https://mangareader.to/read/kaguyasama-love-is-war-13/en/volume-1
```
And enter the final volume you want to download up to (and including):
```
ENTER URL: https://mangareader.to/read/kaguyasama-love-is-war-13/en/volume-1
FINAL VOLUME: 26
```


### Stitching manga into pdf
Now that the manga is downloaded (you can check in the "temp" folder), run stitcher.py and wait for it to generate the pdfs from the downloaded manga, which will be in the downloads folder. 

## NOTE: 
### The get_element to get the number of pages doesn't seem to be intercepted by ads anymore, please open an issue if this causes problems
