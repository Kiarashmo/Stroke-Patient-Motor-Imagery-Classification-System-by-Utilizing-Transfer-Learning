# Stroke Patient Motor-Imagery Classification using Transfer Learning

## Overview
Brain-computer interfaces (BCI), powered by the classification of brain signals such as electroencephalography (EEG), can potentially revolutionize how we interact with computers and the world around us. One of the main applications of these systems is to be used with Motor Imagery (MI) data, in order to detect the movement imagination of a subject without any actual movement, which can then be employed to recover the motor ability of stroke patients, by enabling control of assistive devices like robotic arms. However, a significant challenge in studying stroke patients lies in the scarcity of available MI data.

Given the abundance of large-scale and accessible datasets from healthy subjects, we aimed to investigate whether a model trained on healthy individuals' brain data could help overcome the shortage of stroke patients' data and improve the classification of their imagery movements. To address this, we formulated the problem as a binary hand movement imagery classification task, focusing on distinguishing between imagining the opening and closing of the left or right fist. In the beginning, we utilized EEGNet as the base model of our pipeline and trained it initially on healthy subjects’ motor imagery dataset. Following this initial training, we employed transfer learning techniques and fine-tuned the model for our stroke patients dataset.

## Our Task
Classify whether the brain signal corresponds to the left or right hand

## Results
Our initial results suggest that our method achieved an accuracy of 90% on the healthy dataset. However, the accuracy observed on the stroke patient dataset was average. We anticipate seeing enhanced results after doing some improvements in preprocessing and hyperparameter tuning. In addition, we would like to explore the effect of the EEG channel selection on the model performance and also experiment with a subject-specific transfer learning model.

## Datasets
- Normal MI (Source dataset): [EEG Motor Movement/Imagery Dataset (EEGMMI)](https://physionet.org/content/eegmmidb/1.0.0/)
- Stroke MI (Target dataset): [EEG datasets of stroke patients (Figshare)](https://figshare.com/articles/dataset/EEG_datasets_of_stroke_patients/21679035/3)

## Project Structure
- `notebooks/`: Jupyter notebooks detailing data preprocessing, model training, visualizations, and evaluation.
- `models/`: Saved model weights and architecture configurations for reproducibility.
- `results/`: Outcome metrics, and comparisons with baseline methods.
- `documentation/`: Detailed project documentation, including research papers and presentation materials.

## Contribution
We welcome contributions to this project that can help advance the classification of motor-imagery movements for stroke patient rehabilitation. If you have any suggestions or improvements, please feel free to submit a pull request.

## License
This project is licensed under the MIT License(LICENSE).

## Acknowledgments
We extend our gratitude to the Neuromatch Academy and the community for their support and inspiration during the development of this project.
