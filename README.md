# mazin-ayman-portofolio.github.io
```
from bs4 import BeautifulSoup

import bs4

import requests

seat_number = 15102

url = f"https://natiga4dk.net/fayoum/?type=num&k={seat_number}"

request = requests.get(url)

soup = BeautifulSoup(request.content, 'lxml')

panel = soup.find('div', {'class': 'panel'})

trs: bs4.element.Tag = panel.find_all('tr') # pyright: ignore

data = {

    "name": ,

    "seat_number": seat_number,

    "total": ,

    "percentage": ,

    "main": {

        "arabic": ,

        "english": ,

        "algebra": ,

        "engineering": ,

        "math_total": ,

        "science": ,

        "social_studies": 

    },

    "not_added": {

        "religion": ,

        "art": ,

        "computer": 

    }

}
```
