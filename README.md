# Description
To automate the process of reviewing financial documents by extracting relevant information and generating a report in a question-answer format.

This project aims to automate the process of report generation by making use of two modules - question generation from text and answer extraction from text. Firstly, question extraction modules are used to generate a set of generic questions from a training corpus of financial documents. This generated questions are fed to the test document and answer extraction modules extract the answers for these questions. The question-answer pairs are compiled in the form of a report. We also use the novel idea of using training documents to obtain a set of questions and use the knowledge gained during this for answer extraction. We also generate a generalized set of financial specific questions that can be commonly used across any similar test financial data. 

# Environment
* Docker ver. 17.03+:
  Ubuntu: https://docs.docker.com/engine/installation/linux/ubuntu/#install-using-the-repository
  Mac: https://download.docker.com/mac/stable/Docker.dmg
* Docker-compose ver. 1.13.0+: https://docs.docker.com/compose/install/
* Python 3
* pyzmq dependencies: Ubuntu sudo apt-get install libzmq3-dev or for Mac brew install zeromq --with-libpgm

## Getting Started
Run the setup.ipynb on Jupyter notebook. 

## Deployment
The input can be given as *Input.pdf* (a sample is given, can be overwritten). A set of generalized questions are generated from this file. Questions from multiple such files can be combined. The test file for which summarization in the form of question answers is needed is given as *Test.pdf*. Answers for the generlized questions are generated from this file and given as a form of summarization.

## Authors
* Madhav Sankar K [madhavsankar](https://github.com/madhavsankar)
* Hariharan J 
* Vishal Veda Vyas P 

## Acknowledgments
Thanks to Neural Networks and Deep Learning lab, MIPT for the inspiration for the [Question Generation module](https://github.com/deepmipt/question_generation) and [Answer Extraction module](https://github.com/deepmipt/DeepPavlov).

