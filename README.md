# ML 101

This repository contains the materials of the classes from the UNAVE ML 101 course (2022).
The course is divided into seven different parts:
1. Refresher
2. Data Pre-Processing
3. Classical ML Models
4. Model Evaluation and Validation
5. Clustering
6. Deep-learning
7. Text and Stream Mining

## Google Drive

In this [link](https://drive.google.com/drive/folders/1VK--DpQymu4Tps1KHiXz8Kf4xZd8Pljk?usp=sharing) you have access to the material of the class in a shared google drive folder.

## Slides

1. [Refresher](https://docs.google.com/presentation/d/1bIVQqsFho6R5_NAm1T9mJcf2izAfJ-s0YFSYAawtRK0/edit?usp=sharing)
2. [Pre-processing](https://docs.google.com/presentation/d/156ov7qr4cQVAf8-YjixzLS7fmLXyzSocDYgknWXh4r8/edit?usp=sharing)
3. [Models](https://docs.google.com/presentation/d/1gsC41er8qtMgEEW6ueTHIGDie4QrdYN1g-aiZylCGOw/edit?usp=sharing)
4. [Evaluation](https://docs.google.com/presentation/d/1ELoYLUUmBiNJlrzDyWLFk_2PePY043sssdpqC1y6dOg/edit?usp=sharing)
5. [Unsupervised](https://docs.google.com/presentation/d/1g1ElQcqY_F0R2JlQODzrIXOOKB6q1j_1xqIsTLQEl6I/edit?usp=sharing)
6. [Deep Learning](https://docs.google.com/presentation/d/1OpgIDxLE89a4mpDfIscUfcR2SIdewfCeaLiPaiMJBbE/edit?usp=sharing)
7. [Time Series](https://docs.google.com/presentation/d/1FNP6eKG5apjkY9cUoQTqAciQLPZ2udeQB2kToCx817Q/edit?usp=sharing)/[Text Mining](https://docs.google.com/presentation/d/1VLIScw8gq20uR1KPRBLA-Ni_q0IyiCaYTFlJa4yUHN4/edit?usp=sharing)

## Setup

All of the materials were written in python, using the commonly used libraries.
The materials themselves are organized in Jupyter Notebooks to ease the execution of the same. 
To set up the environment, execute the following commands:

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
jupyter-notebook 
```

### Setup for local Colab

The time series project needs access to the local network to publish the predictions within a local MQTT server.
To achieve this, we can run the colab on a local instance.
Follow this steps to prepare the local virtual environment:

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
jupyter serverextension enable --py jupyter_http_over_ws
jupyter notebook \
  --NotebookApp.allow_origin='https://colab.research.google.com' \
  --port=8888 \
  --NotebookApp.port_retries=0
```


## Authors

* **M??rio Antunes** - [mariolpantunes](https://github.com/mariolpantunes)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
