# Key_Detection

* Before proceding with the problem statement, it will be mindfull to go through [this article](https://stackoverflow.com/questions/3141927/algorithms-for-determining-the-key-of-an-audio-sample) which includes a thread of discussion over the same problem that we are trying to solve and the [Krumhansl-Schmuckler Key-Finding Algorithm](https://www.jstor.org/stable/40285812).
* Lastly, there is also an app [mixxxdj](https://mixxx.org/) which uses a key finder and I managed to find the repository which contains the code for the same and can be found [here](https://github.com/mixxxdj/libkeyfinder).
  
I found and testing two methods to detect the global key or pitch of an audio file:-
### [pyacaKey.py](https://github.com/arnav8/Key_Detection/blob/main/pyacaKey.py):
* Computes the musical key of an input audio file using the idea behind [Krumhansl-Schmuckler Key-Finding Algorithm](https://www.jstor.org/stable/40285812).
* Uses the [pyaca](https://pypi.org/project/pyACA/) python package, which is actually the python scripts accompanying the book [An Introduction to Audio Content Analysis](www.AudioContentAnalysis.org).

### [mmKey.py](https://github.com/arnav8/Key_Detection/blob/main/mmKey.py): 
* Uses a Convolutional Neural Network to detect the global key of the audio file as described in the research paper [Filip Korzeniowski and Gerhard Widmer,
    "Genre-Agnostic Key Classification with Convolutional Neural Networks",
    In Proceedings of the 19th International Society for Music Information 
    Retrieval Conference (ISMIR), Paris, France, 2018.](https://arxiv.org/pdf/1808.05340.pdf).
* This implementation uses a python package called [madmom](https://pypi.org/project/madmom/) and has no other dependencies.



