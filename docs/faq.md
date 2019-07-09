# Frequently Asked Questions

* [Why is there a difference in the numbers reported here and those in the paper?](#why-is-there-a-difference-in-the-numbers-reported-here-and-those-in-the-paper)
* [Why is there silence in some waveforms?](#why-is-there-silence-in-some-waveforms)
* [I found an issue in one or more utterances. How can I report it?](#i-found-an-issue-in-one-or-more-utterances-how-can-i-report-it)
* [What is this data repository being used for?](#what-is-this-data-repository-being-used-for)
* [How can I cite UltraSuite?](#how-can-i-cite-ultrasuite)



------

#### Why is there a difference in the numbers reported here and those in the paper?

Some of the numbers describing the repository in the paper, such as number of utterances or number of speech hours, were estimated at the time of the submission. We are actively working on improving UltraSuite, which means these number might change.

For example, estimates for speech hours (child or therapist speech and silence) may change due to different speaker labelling methods or the removal of identifiable information. The number of utterances may change if we find unusable utterances (poor recording or corrupted data).

To keep track of these changes, please be aware of version numbers in the datasets and their respective labels.

#### Why is there silence in some waveforms?

Some utterances contain regions of artificial silence. These correspond to regions originally containing identifiable information (such as children's names) and speech from additional speakers (such as parent speech). To remove such data, we have replaced them with silence in the waveform.

#### I found an issue in one or more utterances. How can I report it?

Please see [Contributing](index.md#Contributing).

#### What is this data repository being used for?

You can find out the various applications of this data by having a look at [papers that cite Ultrasuite](<https://scholar.google.com/scholar?cites=9159984300116881095&as_sdt=2005&sciodt=0,5&hl=en>). If you are using the repository or know of any applications not listed in the link above, please get in touch with us. We would be happy to hear about it!

#### How can I cite UltraSuite?

For the current release of UltraSuite, if using data or code, please provide appropriate web links and cite the following paper:

- Eshky, A., Ribeiro, M. S., Cleland, J., Richmond, K., Roxburgh, Z.,  Scobbie, J., & Wrench, A. (2018) **Ultrasuite: A repository of ultrasound and acoustic data from child speech therapy sessions**. Proceedings of INTERSPEECH. Hyderabad, India.

If you are using automatically-generated labels, you may also like to cite the following paper:

- Ribeiro, M. S., Eshky, A., Richmond, K. & Renals, S., (2019). **Ultrasound tongue imaging for diarization and alignment of child speech therapy sessions**. Proceedings of INTERSPEECH. Graz, Austria.