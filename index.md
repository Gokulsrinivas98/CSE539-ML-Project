# Sign language interpretation using Deep Learning

## Team Members
- Jayamoorthy, Ajith Kumar
- Srinivasan, Gokul 
- Varatharajan, Akaash
- Venkataramanan, Rohith

## Function of our tool:
Our software aims to translate sign language into English text that would enable easy and efficient communication for aurally impaired people. Communication through sign language will be translated to English in real-time by taking a video stream of sign language as input and classifying
it into textual output using word-level sign recognition. 

## Why we need it and who will benefit from it:
The American Sign Language is one of the most used languages in the United States and is also the fourth- most studied second language in American universities. There are 500,000 ASL users in the US and Canada. In addition to ASL being primarily used by deaf and mute people, ASL is also used by children, siblings, and relatives of deaf people, hearing adults who are becoming
deaf, and a growing population of hearing adults that learn ASL as a second or third language. In addition, ASL improves the quality of family communication for hearing people with deaf and mute relatives.
This Project aims to help reduce the gap between the ASL users and non-ASL users, by helping the non-ASL users learn ASL by practicing it at their own pace. Being an educational tool, everyone that wants to learn ASL would benefit from it.
Furthermore, other applications for this project are:
- Caption generation for Zoom video calls and YouTube sign language content
- Google search using sign language and translations

## Methodology:
The idea is to use a combination of Convolutional Neural Networks (CNN) and Recurrent Neural
Networks (RNN) for video classification. The WLASL dataset holds both RGB video and body key
point data for over 2000 common words, that can be exploited by deep learning algorithms to
learn to classify various hand gestures. CNNs are widely used to recognize and classify images
and are particularly successful at capturing spatial dependencies in an image. On the other hand,
RNNs are adept at learning from sequential and temporal data (e.g., Key points in videos).


The advantages of both these artificial neural networks can be achieved by using the pooling
layer output of CNN as input to the RNN while training. This sequentially passes the convoluted
image features to the RNN, which in turn is expected to make more precise predictions as
compared to a standalone RNN model.
The following steps are proposed to train and test the model:
- Downloading and preprocessing the dataset (Downloading raw videos and extracting
video samples, body key points, etc.).
- Splitting dataset into training and testing data
- Training CNN part of the architecture using TensorFlow
- Store predicted results of the pooling layer of the trained CNN for the training data.
- Use the pooling layer of the CNN as input and train the RNN part of the architecture.
- Testing the architecture using the pooling layer predictions of the trained CNN as inputs
for the RNN.

## Resources used:
- Dataset: Word-Level American Sign Language (WLASL) dataset
- TensorFlow: https://www.tensorflow.org/tutorials/images/cnn

## Demo
[ ]

You can use the [editor on GitHub](https://github.com/Gokulsrinivas98/CSE539-ML-Project/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Gokulsrinivas98/CSE539-ML-Project/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
