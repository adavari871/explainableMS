# Uncovering convolutional neural network decisions for diagnosing multiple sclerosis on conventional MRI using layer-wise relevance propagation

***Fabian Eitel, Emily Soehler, Judith Bellmann-Strobl, Alexander U. Brandt, Klemens Ruprecht, René M. Giess, Joseph Kuchling, Susanna Asseyer, Martin Weygandt, John-Dylan Haynes, Michael Scheel, Friedemann Paul, Kerstin Ritter***

Preprint available [here](https://arxiv.org/abs/1904.08771)

***Abstract:*** Machine learning-based imaging diagnostics has recently reached or even superseded the level of clinical experts in several clinical domains. However, classification decisions of a trained machine learning system are typically non-transparent, a major hindrance for clinical integration, error tracking or knowledge discovery. In this study, we present a transparent deep learning framework relying on convolutional neural networks (CNNs) and layer-wise relevance propagation (LRP) for diagnosing multiple sclerosis (MS), the most widespread autoimmune neuroinflammatory disease. MS is commonly diagnosed utilizing a combination of clinical presentation and conventional magnetic resonance imaging (MRI), specifically the occurrence and presentation of white matter lesions in T2-weighted images. We hypothesized that using LRP in a naive predictive model would enable us to uncover relevant image features that a trained CNN uses for decision-making. Since imaging markers in MS are well-established this would enable us to validate the respective CNN model. First, we pre-trained a CNN on MRI data from the Alzheimer's Disease Neuroimaging Initiative (n = 921), afterwards specializing the CNN to discriminate between MS patients and healthy controls (n = 147). Using LRP, we then produced a heatmap for each subject in the holdout set depicting the voxel-wise relevance for a particular classification decision. The resulting CNN model resulted in a balanced accuracy of 87.04% and an area under the curve of 96.08% in a receiver operating characteristic curve. The subsequent LRP visualization revealed that the CNN model focuses indeed on individual lesions, but also incorporates additional information such as lesion location, non-lesional white matter or gray matter areas such as the thalamus, which are established conventional and advanced MRI markers in MS. We conclude that LRP and the proposed framework have the capability to make diagnostic decisions of CNN models transparent, which could serve to justify classification decisions for clinical review, verify diagnosis-relevant features and potentially gather new disease knowledge.

## Citation
If you found our paper or code relevant to your work, please cite our paper ([preprint](https://arxiv.org/abs/1904.08771)):

```
@misc{Eitel2019Uncovering,
  Author = {Fabian Eitel and Emily Soehler and Judith Bellmann-Strobl and Alexander U. Brandt and Klemens Ruprecht and René M. Giess and Joseph Kuchling and Susanna Asseyer and Martin Weygandt and John-Dylan Haynes and Michael Scheel and Friedemann Paul and Kerstin Ritter},
  Title = {Uncovering convolutional neural network decisions for diagnosing multiple sclerosis on conventional MRI using layer-wise relevance propagation},
  Year = {2019},
  Eprint = {arXiv:1904.08771},
  url = {https://arxiv.org/abs/1904.08771}
}
```


## License
Code is published under the BSD License 2.0.
