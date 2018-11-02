# UXTD - Ultrax Typically Developing Children

#### A dataset of ultrasound and audio recordings from typically developing children



## Speakers

The UXTD dataset contains 58 speakers (31 female and 27 male), aged  5-12 years.

For a list and additional details, see [UXTD Speakers](uxtd-spk.md).

## Data Types

**<u>Core data types</u>**

| Data type | Description                                       |
| --------- | ------------------------------------------------- |
| wav       | speech waveform                                   |
| ult       | raw ultrasound data                               |
| param     | ultrasound parameters                             |
| txt       | prompt text with date/time of utterance recording |

**<u>Additional data</u>**

All labels are provided in Praat's TextGrid format.

| Data type      | Description                                                  |
| -------------- | ------------------------------------------------------------ |
| transcriptions | transcription for utterances of type X and X.                |
| slt-labels     | manual annotation from SLT, when available. See [2] for details |
| speaker-labels | speaker diarization identifying therapist (SLT) and child (CHILD) speech |
| word-labels    | automatic word-level alignment                               |
| phone-labels   | automatic phone-level alignment                              |

## File IDs

Individual recordings are indexed for each session according to their recording times.
See the prompt text file for recording date/time. 

Each file ID also includes a prompt type identifier. See [Data](data.md) for details.

## Download

*Download links will be made available soon*

## References

[1] Eshky, A., Ribeiro, M. S., Cleland, J., Richmond, K., Roxburgh, Z.,  Scobbie, J., & Wrench, A. (2018) **Ultrasuite: A repository of ultrasound and acoustic data from child speech therapy sessions**. Proceedings of INTERSPEECH. Hyderabad, India.

[2] Cleland, J., Scobbie, J., Naki, S., & Wrench, A. (2015). **Helping children learn non-native articulations: the implications for ultrasound-based clinical intervention.** Proceedings of the 18th International Congress of Phonetic Sciences : ICPhS 2015. ed. / The Scottish Consortium for ICPhS 2015. 1. ed. Scotland, 2015. p. 1-5 698.
