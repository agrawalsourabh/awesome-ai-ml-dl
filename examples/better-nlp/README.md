# Better NLP

This is a wrapper program/library that encapsulates a couple of NLP libraries that are popular among the AI and ML communities.

Examples have been used to illustrate the usage as much as possible. Not all the APIs of the underlying libraries have been covered.

The idea is to keep the API language as high-level as possible, so its easier to use and stays human-readable.

Libraries / frameworks covered:

- SpaCy ([site](https://spacy.io/) | [docs](https://spacy.io/usage/))
- Textacy ([github](https://github.com/chartbeat-labs/textacy) | [docs](https://chartbeat-labs.github.io/textacy/))
- nltk ([site](http://www.nltk.org/) | [docs](https://buildmedia.readthedocs.org/media/pdf/nltk/latest/nltk.pdf))

Non-NLP related libraries / frameworks used:
- numpy ([site](https://www.numpy.org/) | [docs](https://docs.scipy.org/doc/))
- networkx ([site](https://networkx.github.io/) | [docs](https://networkx.github.io/documentation/stable/index.html))

## Requirements

- Python 3.7.x or higher
- Docker (optional)
- Diskspace: 2-3GB

## Get started

### Linux / MacOS (Docker environment)

- Clone the repo: `git clone https://github.com/neomatrix369/awesome-ai-ml-dl`
- `cd /path/to/awesome-ai-ml-dl/examples/better-nlp`
- Ensure the Docker daemon is running in the background
- Run `runDockerImage.sh`
- Wait for the docker image to download (first time, one-off)
- Wait for the container to get started with the JuPyter notebook running
- Copy the notebook's url published in the console, should be of the form `http://....?token....)` - you will have to do a tiny bit of amendment to make the url look like `http://localhost:8888?token....`
- Go to the browser and paste the corrected url: `http://localhost:8888?token....`, you should see the screen as described in [Jupyter Notebook](./docs/Jupyter_notebook.md).

### Linux / MacOS (local environment)

- Clone the repo: `git clone https://github.com/neomatrix369/awesome-ai-ml-dl`
- `cd /path/to/awesome-ai-ml-dl/examples/better-nlp/build`
- Run `install-linux.sh` or `install-macos.sh` depending on the OS you are running on
- Run `install-dependencies.sh`
- Run `cd ..`
- Run `jupyter-lab notebooks/jupyter/better_nlp_spacy_texacy_examples.ipynb`
- Wait for the JuPyter lab to open in the browser
- You should see the screen as described in [Jupyter Notebook](./docs/Jupyter_notebook.md).

In theory, the above should work for Windows as well, if run via `git-bash` or `cgywin` with all the necessary requirements installed and available - although it has not been tested, please provide feedback or fixes if you find any.

### Notebooks

#### Jupyter

See [Jupyter Notebook](./docs/Jupyter_notebook.md) 

#### Google Colab

You can open these notebooks directly into Google Colab:
- [better_nlp_spacy_texacy_examples.ipynb](./notebooks/google-colab/better_nlp_spacy_texacy_examples.ipynb) 
- [better_nlp_summarisers.ipynb](./notebooks/google-colab/better_nlp_summarisers.ipynb)

## Installation

Setup an environment needed to be able to run these programs without having to worry about the dependencies they use.

Please be aware that even though we are install only a few components, the installation process takes some time (irrespective if you are running in via your local environment or inside a docker container). Give it about 20-30 minutes depending on network bandwidth and overall machine performance. Or you can use a pre-built docker image, see [Docker environment](README.md#docker_environment.md) for more details.

### Local environment

For the brave at heart, install the dependencies in your local environment.

#### Linux

```bash
./install-linux.sh
```

#### MacOS

```bash
./install-macos.sh
```

Alternatively please refer to the **Docker environment** section.

#### Windows

In principle, the `install-linux.sh` script should work in the `cygwin` or `git bash` environments - although it has not been tested, please raise PR with fixes if any. Alternatively please refer to the **Docker environment** section.

### Docker environment

See [Docker environment](./docs/Docker_environment.md)

## Example code

See [Examples and results](./docs/Examples.md)