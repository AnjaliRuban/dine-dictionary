# Mother Tongues Dictionary for Diné
### Data Not Included

This is based on the starter kit for building a [Mother Tongues Dictionary](https://www.mothertongues.org).

Please visit the [repo](https://github.com/MotherTongues/mothertongues) or [docs](https://docs.mothertongues.org) for more information.


## Setup

First, install the prereqs for this project.


- **Git**: Follow the instructions [here](https://github.com/git-guides/install-git).
- **Python 3.8+**: Follow the instructions [here](https://www.python.org/downloads/).
- **NodeJS 16+**: `pip install nodejs`

First, _clone_ this repo into your computer using the following command.

```
git clone --recurse-submodules --remote-submodules https://github.com/AnjaliRuban/dine-dictionary
```

Now you should have all the files you need except the data files, which have been omitted for privacy.

To make sure everything shows up when we run our code, we want to initalize the user interface.

```
cd mothertongues/mothertongues-UI
npm install
npx nx build mtd-mobile-ui --configuration=pydev
```

Next, install the mothertonuges project itself.

```
cd ..
pip install --editable .
```
Now the command `mothertongues` is available through the terminal.

To run the local version of the dictionary, navigate to the top of our repo (using `cd ..`) and run the following. Make sure you have put your `data.xlsx` file in the folder!

```
c
```

Openning up any brower and navigating to `http://localhost:3636` should pull up your dictionary!


## License

[MIT © Aidan Pine.](LICENSE)
