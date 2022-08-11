# Open Research Challenge - Video analysis & statistics

## Annotation format and labeling instructions
Please have a look into the provided PDF: [Open_Research_Challenge_-_Labeling_Instruction.pdf](https://docs.google.com/viewer?url=https://raw.githubusercontent.com/RoboCup-SPL/Datasets/master/RoboCup%202022/Open%20Research%20Challenge%20-%20Video%20analysis%20%26%20statistics/Open_Research_Challenge_-_Labeling_Instruction.pdf)

## Contributions at the RoboCup 2022
https://spl.robocup.org/rc2022/#open-research-challenge

## Download script

The download script populates the subdirectories by loading images and GameController/TCM log files from the RoboCup cloud server according to the `index.yml` file.

### Requirements
- click
- PyYAML

### Execution

**Warning: This takes a lot of time (unfortunately without progress bar) and disk space (~13.2GB).**

The following command downloads all sub-datasets and extracts them to their respective subdirectories:
```bash
./download.py --extract
```

Instead of downloading the entire dataset, you can also download only specific teams' data:
```bash
./download.py --extract "Berlin United" RoboEireann
```
