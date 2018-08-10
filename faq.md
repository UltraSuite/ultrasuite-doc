# Frequently Asked Questions

* [Why is there a difference in the numbers reported here and those in the paper?](#why-is-there-a-difference-in-the-numbers-reported-here-and-those-in-the-paper)
* [Why is there silence in some waveforms?](#why-is-there-silence-in-some-waveforms)
* [I found an issue in one or more utterances. How can I report it?](#i-found-an-issue-in-one-or-more-utterances-how-can-i-report-it)
* [How can I interpret ultrasound parameters?](#how-can-i-interpret-ultrasound-parameters)
* [How can I cite UltraSuite?](#how-can-i-cite-ultrasuite)



------

#### Why is there a difference in the numbers reported here and those in the paper?

Some of the numbers describing the repository in the paper, such as number of utterances or number of speech hours, were estimated at the time of the submission. We are actively working on improving UltraSuite, which means these number might change.

For example, estimates for speech hours (child or therapist speech and silence) may change due to different speaker labelling methods or the removal of identifiable information. The number of utterances may change if we find unusable utterances (poor recording or corrupted data).

To keep track of these changes, please be aware of version numbers in the datasets and their respective labels.

#### Why is there silence in some waveforms?

Some utterances contain regions of artificial silence. These correspond to regions originally containing identifiable information (such as children's names) and speech from additional speakers (such as parent speech). To remove such data, we have replaced them with silence in the waveform.

#### I found an issue in one or more utterances. How can I report it?

Please see **Contributing <add-link>**.

#### How can I interpret ultrasound parameters?

TODO

#### How can I cite UltraSuite?

For the current release of UltraSuite, if using data or code, please provide appropriate web links and cite the following paper:

- Eshky, A., Ribeiro, M. S., Cleland, J., Richmond, K., Roxburgh, Z.,  Scobbie, J., & Wrench, A. (2018) **Ultrasuite: A repository of ultrasound and acoustic data from child speech therapy sessions**. Proceedings of INTERSPEECH. Hyderabad, India.

