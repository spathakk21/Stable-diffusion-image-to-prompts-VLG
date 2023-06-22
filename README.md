# Stable-diffusion-image-to-prompts-VLG
Made a Image to Text Generator model which is tries to caption AI generated Images.

**MODEL :-** Used a pre-trained **GiT(GenerativeImage2Text)** from hugging face. 

Huggingface link --> https://huggingface.co/microsoft/git-base.

You can learn more about the GiT model by checking links given below -->

GiT Paper :- **A Generative Image-to-text Transformer for Vision and Language**: https://arxiv.org/abs/2205.14100

Documentation :- https://huggingface.co/docs/transformers/model_doc/git

**DATA :-** 

Fine tuned the model by training it on :- **DiffusionDB dataset** which is first large-scale text-to-image prompt dataset.
It contains 14 million images generated by Stable Diffusion using prompts and hyperparameters specified by real users but I **only used subset of 2m_first_1k datapoints** due to less computational power.

Link for DiffusionDB dataset --> https://huggingface.co/datasets/poloclub/diffusiondb/viewer/2m_first_1k/train

**TRAINING :-** 

Trained model for **10 epochs** and saved my tuned model on PC and then again used it for inference.

Unable to load trained model in repository due to excessive size.

**Code Assistance :-** 

I used some of the functions and architecture of code from the following notebook on kaggle --> https://www.kaggle.com/code/thedevastator/blip-large-training-inference/notebook
