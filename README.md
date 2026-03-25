# EE200 End-Semester Project — Audio and Signal Processing

End-semester project for EE200 (Introduction to Signals and Systems) at IIT Kanpur, focusing on frequency mixing and de-mixing using digital signal processing techniques.

## Overview

This project addresses two complementary signal processing problems:

1. **Frequency Mixing (Q1):** Given a set of individual audio signals, construct a combined signal that encodes multiple frequency components together — simulating how signals can be multiplexed for transmission or storage.

2. **Frequency De-mixing (Q2):** Given a mixed audio signal containing contributions from multiple frequency components, isolate and reconstruct the individual constituent signals — equivalent to the inverse multiplexing or channel separation problem.

Both problems are solved using Fourier analysis and filter design. The project includes a demonstration with a real audio file: a piece of music mixed with two piccolo instruments (`song_with_2piccolo.wav`), which is de-mixed to produce a restored output (`restored_song.wav`).

## Repository Structure

| File | Description |
|---|---|
| `EE200_Q1.ipynb` | Notebook implementing the frequency mixing pipeline |
| `EE200_Q1_Report.pdf` | Report detailing the Q1 methodology and results |
| `EE200_Q2.ipynb` | Notebook implementing the frequency de-mixing pipeline |
| `EE200_Q2_Report.pdf` | Report detailing the Q2 methodology and results |
| `Dataset/song_with_2piccolo.wav` | Input mixed audio file used for de-mixing demonstration |
| `Dataset/cat_gray.jpg` | Auxiliary image used in frequency-domain processing |
| `Dataset/dog_gray.jpg` | Auxiliary image used in frequency-domain processing |
| `restored_song.wav` | Output audio file after de-mixing |

## Requirements

- Python 3.8+
- NumPy
- SciPy (`scipy.signal`, `scipy.fft`)
- Matplotlib
- Librosa (audio I/O)

Install with:

```bash
pip install numpy scipy matplotlib librosa
```

## References

- Oppenheim, A.V. and Schafer, R.W. *Discrete-Time Signal Processing.* Prentice Hall.
- EE200 Course Material, IIT Kanpur.
