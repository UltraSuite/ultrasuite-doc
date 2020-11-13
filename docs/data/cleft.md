# The Cleft Palate Dataset

**A dataset of ultrasound and audio recorded with children with cleft lip and palate**

The cleft dataset is a collection of ultrasound tongue imaging 
and audio data, gathered from children with cleft lip and palate 
by a research speech and language therapist working in a hospital
environment.

### Speakers

We recorded data with 39 English-speaking children, but only 29 gave consent to share their data.
These are 11 female speakers and 18 male, aged 7-11 years.

| SPEAKER-ID  | GENDER  | AGE-Y  | AGE-M  | AGE  | CLEFT-TYPE  | OTHER-MEDICAL  |
| ----------- | ------- | ------ | ------ | ---- | ----------- | -------------- |
| 01M | M | 10 | 5 | 10.42 | BCLP | no |
| 03F | F | 5 | 1 | 5.83 | UCLP | no |
| 05M | M | 10 | 3 | 10.75 | UCLP | no |
| 06M | M | 9 | 8 | 9.75 | UCLP | no |
| 07M | M | 9 | 2 | 9.75 | UCLP | no |
| 09M | M | 9 | 8 | 9.33 | UCLP | yes |
| 11M | M | 4 | 5 | 4.42 | CP | no |
| 12F | F | 5 | 1 | 5.42 | CP | yes |
| 14F | F | 5 | 0 | 5.33 | BCLP | no |
| 15F | F | 4 | 9 | 4.75 | UCLP | yes |
| 16M | M | 9 | 7 | 9.33 | UCLP | no |
| 17F | F | 4 | 4 | 4.42 | BCLP | no |
| 18F | F | 5 | 1 | 5.25 | UCLP | no |
| 19F | F | 3 | 9 | 3.58 | CP | yes |
| 20F | F | 7 | 5 | 7.75 | CP | no |
| 21M | M | 9 | 1 | 9.5 | CP | no |
| 24M | M | 6 | 5 | 6.33 | CP | yes |
| 25M | M | 4 | 1 | 4.33 | CP | no |
| 26M | M | 4 | 4 | 4.67 | BCLP | no |
| 28F | F | 8 | 9 | 8.58 | BCLP | no |
| 30F | F | 7 | 7 | 7.42 | CP | no |
| 31F | F | 5 | 4 | 5.42 | CP | no |
| 32M | M | 5 | 8 | 5.5 | UCLP | no |
| 33M | M | 6 | 4 | 6.42 | UCLP | yes |
| 34M | M | 5 | 3 | 5.25 | CP | yes |
| 35M | M | 3 | 7 | 3.42 | UCLP | no |
| 36M | M | 5 | 0 | 5.58 | BCLP | no |
| 37M | M | 7 | 0 | 7.58 | BCLP | no |
| 39M | M | 7 | 0 | 7 | CP | yes |

<br/>



### Cleft Palate Types 

| Data type   | Description                                                               |
| ----------- | ------------------------------------------------------------------------- |
| CP          | cleft palate only                                                         |
| UCLP        | unilateral cleft lip and palate affecting one side of the lip and palate  |
| BLP         | bilateral cleft lip and palate affecting both sides                       |

<br/>



### Sessions

Each child recorded an "Assessment" session, and two children recorded a "Therapy" session.

<br/>


### Data Types

**<u>Core data types:</u>**

| Data type   | Description                                       |
| ----------- | ------------------------------------------------- |
| wav         | speech waveform                                   |
| ult         | raw ultrasound data                               |
| param       | ultrasound parameters                             |
| txt         | prompt text with date/time of utterance recording |

Hardware synchronisation failed for this dataset. We release the parameter
File as exported from the AAA software. In [1] we provide automatically 
predicted synchronisation offsets. 

<br/>


**<u>Additional data:</u>**

| Data type                  | Description                                                     |
| -------------------------- | --------------------------------------------------------------- |
| slt_labels                 | manual annotation from SLT, when available. See [2] for details |
| probe_direction_labels     | a label for each utterance indicating whether the probe was in a coronal position (cor) or midsagittal right or let (sag_right, sag_left) |

<br/>

SLT Labels are available in Praat's TextGrid format, and probe_direction_labels is a csv file. 



### File IDs

Individual recordings are indexed for each session according to their recording times.
See the prompt text file for recording date/time. 

Each file ID also includes a prompt type identifier. See [Data](data.md) for details.

<br/>

### References

[1] Eshky, A.,Cleland, J., Ribeiro, M. S., Renals, S. **Automatic audiovisual synchronisation for ultrasound tongue imaging**. (Under revision).

[2] Cleland, J., Lloyd, S., Campbell, L., Crampin, L., Palo, J.-P., Sugden,E., Wrench, A., & Zharkova, N. (2020). **The impact of real-time ar-ticulatory information on phonetic transcription:  ultrasound-aidedtranscription in  cleft lip and  palate speech**. Folia Phoniatrica etLogopaedica, 72, 120–130.