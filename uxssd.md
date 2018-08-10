# UXSSD - Ultrax Speech Sound Disorders

#### A dataset of ultrasound and audio recordings from children with speech sound disorders



## Speakers

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

## Sessions

| Session | Description                                           |
| ------- | ----------------------------------------------------- |
| BL      | Baseline session before therapy (1-2 sessions)        |
| Mid     | Mid-point session, halfway through therapy            |
| Post    | Post-therapy session, immediately after therapy ended |
| Maint   | Maintenance session, some time after therapy ended    |
| Therapy | Therapy sessions                                      |

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
| slt-labels     | manual annotation from SLT, when available. See [2] for details |
| speaker-labels | speaker diarization identifying therapist (SLT) and child (CHILD) speech |
| word-labels    | automatic word-level alignment                               |
| phone-labels   | automatic phone-level alignment                              |

## File IDs

Individual recordings are indexed for each session according to their recording times.
See the prompt text file for recording date/time. 

Each file ID also includes a prompt type identifier. See [Data](data.md) for details.

## Additional Notes

Speaker 05M was subjected to two rounds of therapy, with corresponding Assessment sessions. These are identified as *_round2 in the speaker directory. Therapy sessions for this speaker are indexed chronologically.

## Download

*Download links will be made available soon*

## References

[1] Eshky, A., Ribeiro, M. S., Cleland, J., Richmond, K., Roxburgh, Z.,  Scobbie, J., & Wrench, A. (2018) **Ultrasuite: A repository of ultrasound and acoustic data from child speech therapy sessions**. Proceedings of INTERSPEECH. Hyderabad, India.

[2] Cleland, J., Scobbie, J. M., & Wrench, A. A. (2015). **Using ultrasound visual biofeedback to treat persistent primary speech sound disorders**. Clinical linguistics & phonetics, 29(8-10), 575-597.