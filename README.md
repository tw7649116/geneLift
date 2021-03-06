===================================================================================
## GeneLift

### Gene model transfer from closely related reference genomes using cDNA alignments

===================================================================================
```
## Usage
usage: geneLift.py [-h] -cDNA CDNA -g FAA -func ANNOT [-o OUT_P] [-x]
                   [-aligner ALIGNER] [--report-duplications] [-mm M_PATH]
                   [-gm GM_PATH] [-c 90] [-i 95] [-t 1]

Script to liftover gene models from reference cDNA alignments

optional arguments:
  -h, --help            show this help message and exit
  -cDNA CDNA            fasta file containing transcript sequences
  -g FAA                Assembly fasta file to lift over gene models
  -func ANNOT           Semicolon (;) seperated text file with
                        transcript_id,gene_id,functional annotation for the
                        cDNA file
  -o OUT_P              output directory name
  -x                    enable cross species cDNA alignment ; only supported
                        with aligner gmap
  -aligner ALIGNER      Aligner used for cDNA alignments options:
                        [gmap,minimap2]
  --report-duplications
                        Report gene duplications
  -mm M_PATH            path to minimap2 executable
  -gm GM_PATH           path to gmap executable
  -c 90                 Coverage threshold for transcript alignments
  -i 95                 Identity threshold for transcript alignments
  -t 1                  Number of threads
```
## Installation

### Dependencies

To install the dependencies do ( requires conda : https://docs.conda.io/projects/conda/en/latest/ )
```
git clone https://github.com/srividya22/geneLift.git
cd geneLift
chmod +x ./INSTALL.sh
./INSTALL.sh
```


### Installation
```
$ python setup.py install
```
