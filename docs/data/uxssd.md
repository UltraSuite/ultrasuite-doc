# Ultrax Speech Sound Disorders

**A dataset of ultrasound and audio recordings from children with speech sound disorders**



### Speakers

The UXSSD dataset contains 8 speakers (2 female and 6 male), aged 5-10 years.

The table below give further details for each speaker. Ages were taken in the first Assessment session and are indicated in years (AGE-Y) and months (AGE-M).

| SPEAKER-ID | GENDER | AGE-Y | AGE-M | AGE   |
| ---------- | ------ | ----- | ----- | ----- |
| 01M        | M      | 6     | 0     | 6.0   |
| 02M        | M      | 10    | 1     | 10.08 |
| 03F        | F      | 8     | 7     | 8.58  |
| 04M        | M      | 8     | 11    | 8.92  |
| 05M        | M      | 6     | 5     | 6.42  |
| 06M        | M      | 5     | 11    | 5.92  |
| 07F        | F      | 7     | 6     | 7.5   |
| 08M        | M      | 7     | 7     | 7.58  |

Sessions

| Session | Description                                           |
| ------- | ----------------------------------------------------- |
| BL      | Baseline session before therapy (1-2 sessions)        |
| Mid     | Mid-point session, halfway through therapy            |
| Post    | Post-therapy session, immediately after therapy ended |
| Maint   | Maintenance session, some time after therapy ended    |
| Therapy | Therapy sessions                                      |



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
/uxssd
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



### Additional Notes

Speaker 05M was subjected to two rounds of therapy, with corresponding Assessment sessions. These are identified as *_round2 in the speaker directory. Therapy sessions for this speaker are indexed chronologically.



### References

[1] Eshky, A., Ribeiro, M. S., Cleland, J., Richmond, K., Roxburgh, Z.,  Scobbie, J., & Wrench, A. (2018) **Ultrasuite: A repository of ultrasound and acoustic data from child speech therapy sessions**. Proceedings of INTERSPEECH. Hyderabad, India.

[2] Cleland, J., Scobbie, J. M., & Wrench, A. A. (2015). **Using ultrasound visual biofeedback to treat persistent primary speech sound disorders**. Clinical linguistics & phonetics, 29(8-10), 575-597.

[3] Ribeiro, M. S., Eshky, A., Richmond, K., Renals, S., (2019). **Ultrasound tongue imaging for diarization and alignment of child speech therapy sessions**. Proceedings of INTERSPEECH. Graz, Austria.