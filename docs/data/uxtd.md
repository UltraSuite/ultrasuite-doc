# Ultrax Typically Developing Children

**A dataset of ultrasound and audio recordings from typically developing children**



### Speakers

The UXTD dataset contains 58 speakers (31 female and 27 male), aged  5-12 years.

For a list and additional details, see [UXTD Speakers](uxtd-spk.md).



### Data Types

**<u>Core data types</u>**

| Data type | Description                                       |
| --------- | ------------------------------------------------- |
| wav       | speech waveform                                   |
| ult       | raw ultrasound data                               |
| param     | ultrasound parameters                             |
| txt       | prompt text with date/time of utterance recording |

**<u>Additional data</u>**

| Data type        | Description                                                  |
| ---------------- | ------------------------------------------------------------ |
| transcriptions   | transcription for utterances of type X and X.                |
| slt_labels       | manual annotation from SLT, when available. See [2] for details |
| speaker_labels   | speaker diarization identifying therapist (SLT) and child (CHILD) speech |
| word_labels      | automatic word-level alignment                               |
| phone_labels     | automatic phone-level alignment                              |
| reference_labels | manually-revised labels (see below for details)              |

Labels are available in Praat's TextGrid format and HTK's lab format.

Speaker, word, and phone labels were generated according to the methods described in [3].



### File IDs

Individual recordings are indexed for each session according to their recording times.
See the prompt text file for recording date/time. 

Each file ID also includes a prompt type identifier. See [Data](data.md) for details.



### Reference Labels

Reference labels are given for a few utterances of the UXTD and UXSSD datasets. These have been manually revised at the speaker (60 utterances) and word level (199 utterances). The revision was done by a single annotator.

Note that phone labels are also provided, but these are *not entirely manually-revised*. This set of annotation is force-aligned at the phone level, but constrained by the manually-revised word boundaries.

Labels are available in Praat's TextGrid format (`TG`) and HTK's lab format (`lab`). The structure for the directory is as follows:

```
/uxtd
	/phone_labels
		/lab
		/TG
	/word_labels
		/lab
		/TG
	/speaker_labels
		/lab
		/TG
```



### References

[1] Eshky, A., Ribeiro, M. S., Cleland, J., Richmond, K., Roxburgh, Z.,  Scobbie, J., & Wrench, A. (2018) **Ultrasuite: A repository of ultrasound and acoustic data from child speech therapy sessions**. Proceedings of INTERSPEECH. Hyderabad, India.

[2] Cleland, J., Scobbie, J., Naki, S., & Wrench, A. (2015). **Helping children learn non-native articulations: the implications for ultrasound-based clinical intervention.** Proceedings of the 18th International Congress of Phonetic Sciences : ICPhS 2015. ed. / The Scottish Consortium for ICPhS 2015. 1. ed. Scotland, 2015. p. 1-5 698.

[3] Ribeiro, M. S., Eshky, A., Richmond, K., Renals, S., (2019). **Ultrasound tongue imaging for diarization and alignment of child speech therapy sessions**. Proceedings of INTERSPEECH. Graz, Austria.

