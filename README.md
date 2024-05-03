# Voice-Recognition-with-MFCC
Command Recognition Using MFCC Features

MFCC is a widely used technique for extracting features from audio signals. Firstly, the audio signal undergoes a windowing process, followed by the application of FFT (Fast Fourier Transform) for each window. Then, the resulting power spectrum is scaled according to the Mel scale, which is more suitable for human hearing. This process better reflects how the human ear processes sound.

The spectrum transformed into the Mel scale then undergoes a transformation called cepstrum. Cepstrum is used to represent the temporal changes of spectral features. Subsequently, a process called liftering is applied to reduce local variance among cepstral coefficients. Finally, the obtained coefficients are typically used as vector representations, commonly in applications like command recognition.

MFCC provides a representation of audio signals that is more suitable for human hearing. Therefore, it is widely preferred in applications such as command recognition. The advantages of MFCC include low-dimensional feature vectors, reflecting the characteristics of human hearing, and high recognition accuracy. These features play an important role in enhancing the effectiveness of command recognition systems.


FSK (Frequency Shift Keying) is a modulation technique used in digital communication systems. Essentially, it involves switching between two or more fixed frequencies to convey information. This means that the frequency of the signal is changed to convey information.

Typically, the frequency of a carrier wave is altered based on the digital data being carried. For example, one frequency might be assigned for one state (e.g., a state represented as "1"), while a different frequency might be assigned for another state (a state represented as "0").

FSK modulation is commonly found in many communication protocols used for data transmission. For instance, it is used in wireless communication technologies like Bluetooth and Wi-Fi, in modems over telephone lines, and in various other data transmission systems.

Advantages of FSK modulation include simplicity, resilience, and cost-effectiveness. However, it may have some limitations in applications requiring higher data rates.


In the project, a CNN-based artificial intelligence architecture for command recognition is developed using TensorFlow/Keras in the Python environment. The input data for the artificial intelligence architecture is trained using Mel Frequency Cepstral Coefficients-based 13 features extraction and windowing features of size 512 from the audio recordings. The artificial intelligence architecture receives the recorded audio from the LabVIEW program. Then, using LabVIEW, a sound recording is performed, and the recorded audio is sent to the prediction algorithm through a block. The output of the prediction algorithm is pulled from the Python environment to the LabVIEW environment and sent to the RX part through FSK modulation, where the results are displayed.
