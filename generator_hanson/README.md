# 13

## Molecular generator hands-on

## Authors
- fmkz___, iwatobipen

## Requirements

- python 3.x
- RDKit
- Pytorch ( for OSx < 0.4, for Linx <=0.4 )

## How to start

- Clone REINVENT
```
$ cd <path to your working directory>
$ git clone https://github.com/MarcusOlivecrona/REINVENT.git
```
- Get learned dataset,, unzip and move the folder to REINVENT
```
$ wget https://github.com/Mishima-syk/13/blob/master/generator_hanson/data.zip 
$ unzip data.zip
$ mv data ./REINVENT/
```
- Run the sample code with 'tanimoto query'
- (Large num-steps number requires long CPU times. You need a GPU if you set large step number ;-))
```
$ ./main.py --scoring-function tanimoto --scoring-function-kwargs query_structure 'COc1ccccc1' --num-steps 10
```

## About the data
- This model was trained with 1.1 million SMILES strings which is provided from ChEMBL.
- It tooks several hours for traingin with GPU machine (GTX 1080Ti)

## Acknowledgements
- Marcus Olivecrona, developer of [REINVENT](https://github.com/MarcusOlivecrona/REINVENT)


