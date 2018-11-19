# Face Recognition

Face recognition involves identifying or verifying a person 
from a digital image or video frame and is still one of the most
challenging tasks in computer vision today. The conventional 
face recognition pipeline consists of face detection, face alignment, 
feature extraction, and classification. 

Implementing face verification and recognition efficiently at 
scale presents serious challenges
to current approaches. In this project,  we used a paper published
by Google Facenet for face recognition. It directly learns a mapping from
face images to a compact Euclidean space where distances
directly correspond to a measure of face similarity. Once
this space has been produced, tasks such as face recognition,
verification and clustering can be easily implemented
using standard techniques with FaceNet embeddings as feature
vectors.

This project uses a deep convolutional network trained
to directly optimize the embedding itself, rather than an intermediate
bottleneck layer as in previous deep learning
approaches. To train, we use triplets of roughly aligned
matching / non-matching face patches generated using a
novel online triplet mining method. The benefit of our
approach is much greater representational efficiency: we
achieve state-of-the-art face recognition performance using
only 128-bytes per face.
