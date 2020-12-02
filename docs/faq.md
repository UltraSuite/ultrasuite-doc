# Frequently Asked Questions

* [Why is there a difference in the numbers reported here and those in the paper?](#why-is-there-a-difference-in-the-numbers-reported-here-and-those-in-the-paper)

* [Why is there silence in some waveforms?](#why-is-there-silence-in-some-waveforms)

* [Do you have any notes on synchronisation?](#do-you-have-any-notes-on-synchronisation)

* [Why are some speakers missing from the Cleft dataset?](#why-are-some-speakers-missing-from-the-cleft-dataset)

* [I found an issue in one or more utterances. How can I report it?](#i-found-an-issue-in-one-or-more-utterances-how-can-i-report-it)

* [What is this data repository being used for?](#what-is-this-data-repository-being-used-for)

* [How can I cite UltraSuite?](#how-can-i-cite-ultrasuite)

* [How can I cite the TaL corpus?](#how-can-i-cite-the-tal-corpus)

  

------

#### Why is there a difference in the numbers reported here and those in the paper?

Some of the numbers describing the repository in the initial paper, such as number of utterances or number of speech hours, were estimated at the time of the submission. We are actively working on improving UltraSuite, which means these number might change.

For example, estimates for speech hours (child or therapist speech and silence) may change due to different speaker labelling methods or the removal of identifiable information. The number of utterances may change if we find unusable utterances (poor recording or corrupted data).

To keep track of these changes, please be aware of version numbers in the datasets and their respective labels.

#### Why is there silence in some waveforms?

Some utterances contain regions of artificial silence. This occurs only in the child speech datasets. These correspond to regions originally containing identifiable information (such as children's names) and speech from additional speakers (such as parent speech). To remove such data, we have replaced them with silence in the waveform.

#### Do you have any notes on synchronisation?

For the Tongue and Lips corpus, [these notes might be helpful](data/tal_corpus_sync.md).

#### Why are some speakers missing from the Cleft dataset?

A total of 39 English-speaking children recording data for the cleft data. However, only 29 gave consent for their data to be released. These are 11 female speakers and 18 male speakers. We preserve the original speaker identifiers because it will make it easier to match other published work. For example, Cleland et al (2020) [cited here](data/cleft.md#references).

#### I found an issue in one or more utterances. How can I report it?

Please see [Contributing](index.md#Contributing).

#### What is this data repository being used for?

You can find out the various applications of this data by having a look at [papers that cite Ultrasuite](<https://scholar.google.com/scholar?cites=9159984300116881095&as_sdt=2005&sciodt=0,5&hl=en>). A list of papers is also available [here](community.md#publications). If you are using the repository or know of any applications not listed in these links, please get in touch with us. We would be happy to hear about it!

#### How can I cite UltraSuite?

If you use UXTD, UXSSD, or UPX, please provide appropriate web links and cite the following paper:

- Eshky, A., Ribeiro, M. S., Cleland, J., Richmond, K., Roxburgh, Z.,  Scobbie, J., & Wrench, A. (2018) **Ultrasuite: A repository of ultrasound and acoustic data from child speech therapy sessions**. Proceedings of INTERSPEECH. Hyderabad, India.

If you are using automatically-generated labels, you may also like to cite the following paper:

- Ribeiro, M. S., Eshky, A., Richmond, K. & Renals, S., (2019). **Ultrasound tongue imaging for diarization and alignment of child speech therapy sessions**. Proceedings of INTERSPEECH. Graz, Austria.

#### How can I cite the TaL corpus?

If you use the TaL corpus, please provide appropriate web links and cite the following paper:

- Ribeiro, M. S., Sanger, J., Zhang, J.-X., Eshky, A., Wrench, A., Richmond, K.,& Renals, S. (2021).  **TaL: a synchronised multi-speaker corpus of ultrasound tongue imaging, audio, and lip videos.** Proceedings of the IEEE Workshop on Spoken Language Technology (SLT). Shenzhen, China. [[paper](../papers/tal_corpus_SLT2021.pdf)] 

