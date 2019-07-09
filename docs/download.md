# Download

The complete data from the UltraSuite repository is available via the `rsync` command. All flags from this tool should be valid when syncing the UltraSuite repository.

Sample data from the UltraSuite repository is available via [Edinburgh DataShare](http://hdl.handle.net/10283/3255). 



### Download sample data

Download of a very small subset of the UltraSuite repository can be achieve via [Edinburgh DataShare](http://hdl.handle.net/10283/3255). The downloadable datasets on DataShare contain a small sample from each of the three datasets in the UltraSuite repository, as well as their accompanying documentation. This is convenient for users who are unable or unwilling to download the repository using `rsync`.

This may be the case if you are a Windows user. `rsync` is not trivially installed and manipulated from Windows. Feel free to explore the sample data from Edinburgh DataShare and determine if the UltraSuite repository fit your needs. Please get in touch with us and we'll try and share the complete repository with you.



### Using rsync

`rsync` is a command-line tool that allows efficient and fast transfer and synchronisation of files across systems. This is usually pre-install on Linux or mac machines. These instructions assume you have the tool installed on your system, but do not assume a lot of experience with its usage. 

If you are familiar with `rsync`, you can skip ahead and merely glance at the typical commands. All flags commonly used with the tool should be applicable to this scenario. See the [man page](https://linux.die.net/man/1/rsync) for further details.

If you are not familiar with `rsync`, you should be aware that, if you have a version of the data on your disk, `rsync` will **synchronise** your local data with the latest version of UltraSuite. If there are changes to the UltraSuite repository, your data will be overwritten with those latest changes. A useful flag to use with the tool is `--dry-run`, which will simulate the synchronisation process.

Because the repository is quite large (**380 GB**), please make sure you have enough space on your disk. Alternatively, go through these instructions and download only a subset of the data for which you have space for.



### Setting up

To get started, please create a directory on a hard drive where a large amount of space is available. Then, change your current directory onto that newly created one. On Linux or macOS, this can be achieved by running:

```shell
mkdir UltraSuite
cd UltraSuite
```



### Download an utterance

Now that we have a place to store the data, we will download some sample data from the repository. This might be useful if you wish to get a small example to get familiar with the format of the data or test some code.

We first download a single utterance. This is a set of four files: a waveform (.wav), a text file with the prompt text and recording date time (.txt), the raw ultrasound data (ult), and a text file with parameters for the ultrasound data (.param). Running the following command should sync the first utterance from speaker 01M in the Ultrax Typically Developing (UXTD) data set. 

```shell
rsync -av ultrasuite-rsync.inf.ed.ac.uk::ultrasuite/core-uxtd/core/01M/001* .
```

The sample we've just downloaded should give you an idea of the type of data available in UltraSuite. Speaker 01M in the UXTD set has 121 utterances. You can download different samples by changing `001*` to the corresponding utterance.

If you'd like, you can get all of the data for speaker 01M. This corresponds to **1.9GB**!  To do so, please run the following command

```shell
rsync -av ultrasuite-rsync.inf.ed.ac.uk::ultrasuite/core-uxtd/core/01M .
```



### Download a data set

You can download an entire data set by syncing its corresponding directory. For example, for the UXTD data set (82GB), you can run the following command:

```shell
rsync -av ultrasuite-rsync.inf.ed.ac.uk::ultrasuite/core-uxtd .
```

The same command can be used to download `/core-uxssd` and `/core-upx`. Please be aware that each dataset can be quite large:

| Dataset     | Size  |
| ----------- | ----- |
| /core-uxtd  | 82GB  |
| /core-uxssd | 110GB |
| /core-upx   | 191GB |

The structure of each data set is identical and it follows the following pattern:

```
./core-uxtd
	/doc
	/core
		/01M
		/02M
		...
```

Please see the list of speakers of each of the datasets, if you are interested in downloading data from single speakers. Each speaker directory will contain four data types: waveforms (`.wav`), prompts (`.txt`), ultrasound data (`.ult`), and ultrasound parameters (`.param`) .

To simulate the process, you can run `rsync` with the flag `--dry-run` and get an estimate for the amount of data.



### Download label data

To download manual and automatically-generated labels for all three datasets (~80MB), please run:

```sh
rsync -av ultrasuite-rsync.inf.ed.ac.uk::ultrasuite/labels-uxtd-uxssd-upx .
```

You can get labels for each of the datasets by appending `/uxtd`, `/uxssd`, or `/upx`to the command above. There is also a documentation directory for the labels called `/doc`.

Previous versions of label data are archived in the top-level directory `archive`. To download an earlier version of label data, please run something like:

```sh
rsync -av ultrasuite-rsync.inf.ed.ac.uk::ultrasuite/archive/labels-uxtd-uxssd-upx-1.0.zip .
```

The command above will download version 1.0 of labels. Replace the version number as appropriate.

### Download selected data types

Using `rsync`, it is possible to download only specific data types by specifying the desired extension. For example, you can download waveforms (`.wav`), prompts (`.txt`), ultrasound data (`.ult`), or ultrasound parameters (`.param`) separately. To achieve this, the `rsync`command would look like:

```sh
rsync -av --include="*/" --include="*.wav" --exclude="*" ultrasuite-rsync.inf.ed.ac.uk::ultrasuite/core-uxtd .
```

This command downloads all waveforms from the UXTD dataset. Note that the `--include` flags works together with the `--exclude` flag. It is used to include files that would otherwise be excluded. The way to interpret this command is that we first exclude all files with `--exclude="*"`. Then we include all directories with `--include="*/"` and all files ending with the desired extension with `--include="*.wav"`. Additional include flags may specify other data types, for example `--include="*.txt"` to download all prompts.



### Download the entire repository

The following command illustrates how you can download the entire repository. 

**Warning: running the following command will download ~380GB of data!**

`rsync -av ultrasuite-rsync.inf.ed.ac.uk::ultrasuite .`