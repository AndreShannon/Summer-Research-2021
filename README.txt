Created during the Summer of 2021 at the University of Richmond by Dr. Szajda's Code Sleuths AKA The Arrogant Pricks.
(Mostly Angela Stefanovska, André Shannon, and Nikita Morozov)

We were working on implementing an explanation method for automated voice processing systems, more specifically, adapting LIME to work with DeepSpeech2.

This code was made to run in Google Colab since it's too slow without a GPU.



We left off working on implementing Gaussian Mixture models so we could model the decision boundary like LEMNA does. I believe it still needs work, so I would not trust the Gaussian implementation as is.

About the files and where they were stored on my google drive: 
The .ipynb file were stored in a folder called "Colab Notebooks" in my main directory and I think it was a default folder that google colab created. All the other data such as the csv files we were storing data in and the audio folder containing alignments and speech_commands were in a directory that I choose/created for it.


DiffBins.ipynb:
This code generates the data stored in the .csv files. There are lots of hyper-parameters, including but probably not limited to the binning method, the number of bins, number of perturbations, the modeling method, the maximum amplitude we normalized the samples to, the sigma and distance function we used in the weight function, and the maximum we were going to perturb a sample.

Note: We were manually changing the name of the .csv file we were saving the data to so if you forget to change it, it will have the same name and overwrite the last file that was created.


Graphing coefs.ipynb:
This code graphs the coefficients of the models which are stored in the .csv files.


Data and graphs already generated:
We were constantly changing the code, adding more data to the .csv files, and testing different hyper-parameters during the summer so they might look very different from one another. Some of them were probably also generated while testing something and might not be accurate such as the Gaussian Mixture Model ones.