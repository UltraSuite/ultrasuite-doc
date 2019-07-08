# UltraPhonix

**A dataset of ultrasound and audio recordings from children with speech sound disorders**



### Speakers

TODO



### Sessions

| Session | Description                                                  |
| ------- | ------------------------------------------------------------ |
| Suit    | Suitability session to determine if child needs speech therapy |
| BL      | Baseline session before therapy (1-2 sessions)               |
| Mid     | Mid-point session, halfway through therapy                   |
| Post    | Post-therapy session, immediately after therapy ended        |
| Maint   | Maintenance session, some time after therapy ended           |
| Therapy | Therapy sessions                                             |



### Data Types

**<u>Core data types</u>**

| Data type | Description                                       |
| --------- | ------------------------------------------------- |
| wav       | speech waveform                                   |
| ult       | raw ultrasound data                               |
| param     | ultrasound parameters                             |
| txt       | prompt text with date/time of utterance recording |

**<u>Additional data</u>**

| Data type      | Description                                                  |
| -------------- | ------------------------------------------------------------ |
| slt_labels     | manual annotation from SLT, when available. See [2] for details |
| speaker_labels | speaker diarization identifying therapist (SLT) and child (CHILD) speech |
| word_labels    | automatic word-level alignment                               |
| phone_labels   | automatic phone-level alignment                              |

Labels are available in Praat's TextGrid format and HTK's lab format.

Speaker, word, and phone labels were generated according to the methods described in [4].



### File IDs

Individual recordings are indexed for each session according to their recording times.
See the prompt text file for recording date/time. 

Each file ID also includes a prompt type identifier. See [Data](data.md) for details.



### References

[1] Eshky, A., Ribeiro, M. S., Cleland, J., Richmond, K., Roxburgh, Z.,  Scobbie, J., & Wrench, A. (2018) **Ultrasuite: A repository of ultrasound and acoustic data from child speech therapy sessions**. Proceedings of INTERSPEECH. Hyderabad, India.

[2] Cleland, J., Scobbie, J. M., Heyde, C., Roxburgh, Z., & Wrench, A. A. (2017). **Covert contrast and covert errors in persistent velar fronting**. Clinical linguistics & phonetics, 31(1), 35-55.  

[3] Cleland, J., Scobbie, J. M., Roxburgh, Z., Heyde, C., & Wrench, A. A. (Under Revision).  **Enabling New Articulatory Gestures in Children with Persistent Speech Sound Disorders using Ultrasound Visual Biofeedback**. Journal of Speech, Language, and Hearing Research.

[4] Ribeiro, M. S., Eshky, A., Richmond, K., Renals, S., (2019). **Ultrasound tongue imaging for diarization and alignment of child speech therapy sessions**. Proceedings of INTERSPEECH. Graz, Austria.



