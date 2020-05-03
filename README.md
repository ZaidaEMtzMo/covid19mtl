COVID-19 MTL
============

A simple dashboard to display up-to-date epidemiological data on COVID-19 in Montreal.

View the application at [covid19mtl.ca](https://covid19mtl.ca/en)

I'd be happy to help if you'd like to make a version of this for your own city. You can find my contact info here: [jeremymoreau.com](https://jeremymoreau.com/)

## Running Locally

Here are the steps to follow if you want to run COVID-19 MTL locally for testing or development purposes:

1. Clone this repository then navigate to the checkout
2. Create a virtual environment: `python3.8 -m venv .venv`
3. Activate the environment: `. .venv/bin/activate` (the command is `.`, meaning source or include)
4. Install dependencies: `pip install -r requirements.txt`
5. Run the app!  `python -m app`

## Managing dependencies

We use [pip-tools](https://github.com/jazzband/pip-tools) to make it easy to add or
change dependencies.  Direct dependencies of the app are added to `requirements.in`,
with version specifiers that allow bugfix updates.  The command `pip-compile
requirements.in` writes the full list of all needed packages, with pinned versions,
to the `requirements.txt` file, which is used for deployment.

To add a dependency or change the version of an existing one, edit `requirements.in`
and run `pip-compile`, adapt the code of the app if that's needed, then commit all
changes.

## License

The COVID-19 MTL project is available under the [MIT License](https://github.com/jeremymoreau/covid19mtl/blob/master/LICENSE.txt). The hosted version at https://covid19mtl.ca is [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/), but you are not required to apply this license to forks of this code (though it is encouraged as a CC license will make it clear that anyone is free to copy the plots/images and post them elswhere).

## Contributors

- Chinese translation: [Shangge Jiang](https://ca.linkedin.com/in/shangge-vivien-jiang-83418a117)
- Spanish translation: [Zaida Escila Martínez Moreno](https://github.com/ZaidaEMtzMo)

## Screenshot

![covid19mtl.ca](https://user-images.githubusercontent.com/7446564/80046446-a25c9400-84d8-11ea-8063-c36921049d10.png)
