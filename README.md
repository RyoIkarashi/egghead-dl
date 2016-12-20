# [Egghead.io](https://egghead.io) Video Downloader

NOTE: To download premium videos, you're required to have an egghead.io premium account.


## REQUIREMENTS

python 3.x

### Install requirements

	pip install -r requirements.txt

### Globally install egghead-downloader via npm

	npm install -g egghead-downloader


## USAGE

**Step1:** Edit `config.py` and replace `your username here` and `your password here` with your own.

**Step2:** Edit `cookies.txt` and copy and paste egghead.io site's cookie.
To copy the cookie, I used [cookies.txt](https://chrome.google.com/webstore/detail/cookiestxt/njabckikapfpffapmjgojcnbfjonfjfg?hl=en), a chrome extension.

**Step3:** Excute the command below.

	python dl.py [OPTIONS]

## OPTIONS

	--technology		technology name (default: react)

	--slug			  course slug (default: None)
			  		  it'll be shown as its url.

	--directory		 directory where videos will be added
						e.g. ~/Desktop/eggheadio

## EXAMPLES

Download all courses in egghead.io

	python dl.py

Download a specific course

	python dl.py --slug getting-started-with-react

Download all courses in a specific technology and put them to `~/Desktop/videos/*`

	python dl.py --technology react --directory ~/Desktop

## OUTPUT

Downloaded videos will be stored in
 `./videos/TECHNOLOGY_NAME/COURSE_NAME/INDEX-LESSON_NAME.[ext]`

e.g. `./videos/react/Getting Started with React Router/01-Introduction.mp4`

## Special Thanks

	[SimonSelg](https://github.com/SimonSelg/) - the author of [egghead-downloader](https://github.com/SimonSelg/egghead-downloader)
