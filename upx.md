# UPX - UltraPhonix

#### A dataset of ultrasound and audio recordings from children with speech sound disorders



## Speakers

TODO

## Sessions

| Session | Description                                                  |
| ------- | ------------------------------------------------------------ |
| Suit    | Suitability session to determine if child needs speech therapy |
| BL      | Baseline session before therapy (1-2 sessions)               |
| Mid     | Mid-point session, halfway through therapy                   |
| Post    | Post-therapy session, immediately after therapy ended        |
| Maint   | Maintenance session, some time after therapy ended           |
| Therapy | Therapy sessions                                             |

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

## Download

*Download links will be made available soon*

## References

[1] Eshky, A., Ribeiro, M. S., Cleland, J., Richmond, K., Roxburgh, Z.,  Scobbie, J., & Wrench, A. (2018) **Ultrasuite: A repository of ultrasound and acoustic data from child speech therapy sessions**. Proceedings of INTERSPEECH. Hyderabad, India.

[2] TODO

