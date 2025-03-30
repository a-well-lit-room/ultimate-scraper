# ultimate-scraper
Scrape tabs from ultimate guitar. This project is a fork of [RichVarney's original script](https://github.com/RichVarney/ultimate-scraper), with customizations that simply interactions in the command line.

This script downloads tabs from https://www.ultimate-guitar.com/ and saves them as .txt files.

BeautifulSoup is used to search ultimate guitar for tabs. There is a command line interface to allow the user to perform the search and to choose which tabs to download.

During testing, tabs were being downloaded at around 4-5 tabs per second.

## How to use:
- Run the 'ultimate.scraper.py' script using python 3
- Follow the prompts that ask for user input
- Search results will include guitar tabs, guitar chords, and ukulele chords, and filter out all other types (the original script filters out ukulele chords)
- You can then choose to download individual, a selection, a range, or all tabs
from the search result
    - e.g.:  
        1, 2, 3, 4 (tabs 1, 2, 3 and 4 in the list)  
        1, 2, 6, 8 (tabs 1, 2, 6 and 8 in the list)  
        1-4 (tabs 1 to 4 in the list)  
        2-7 (tabs 2 to 7 in the list)  
        all (all tabs in the list)
- Tabs will be saved as .txt format
- Tabs will be saved in the current working directory


#### Example usage downloading single tabs at a time, from a 'general' search:

```
python /Users/user_name/ultimate-scraper.py

> General search or specific artist/band?
> Options "general" or "artist": general

> Search for: laura marling daisy

[1] Laura Marling - Daisy (Chords) Version 1, rating: 4.8404, votes: 7
[2] Laura Marling - Daisy (Tabs) Version 1, rating: 4.91133, votes: 15

> Pick a tab by entering a number, range or "all": 1

> Download finished
> Location: /Users/user_name/tabs
```

## Requirements:
- Python 3 (3.7.7 was using in testing this project)
- Beautiful Soup (3.2.2 was used in testing this project)

Inspiration for this was taken from [https://github.com/ccabrales/TabHero](https://github.com/ccabrales/TabHero)

## Contributing
Pull requests are welcome, however, I will not be looking at this frequently. For major changes, please open an issue first to discuss what you would like to change.

## License
[MIT](https://choosealicense.com/licenses/mit/)
