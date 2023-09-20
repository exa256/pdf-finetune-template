## Template: Finetune OpenAI Model on PDF 

This notebook show an example for finetunning AI model on an arbitrary local PDF
This is a fork from [Llama Index OpenAI Finetunning notebook](https://github.com/jerryjliu/llama_index/blob/main/docs/examples/finetuning/openai_fine_tuning.ipynb), albeit without eval and training/validation sets split.

## Requirements
using python version 3.11.x

## Set up with VSCode
1. move the pdf to train underneeth the ./data
2. install needed dependencies `pip install requirements.txt`
3. on VSCode: download Python and Jupyter notebook extension

## Running the notebook
refer to the notebook and run each cells sequentially. Do note that depending on the number of questions, model for synthetic data set generation, and length of the PDF- the wait time can be significant.

example on a 260 pages PDF book takes 3 hours to generate data sets, and ~1 hour to fine tune.

## Testing
original llama index example contains automated testing and validation, but this is not necessary.

Easiest way to test is to go to the [Playground UI](https://platform.openai.com/playground).
After the job is done, there should be a drop down to select the new fine-tuned model for conversation.
