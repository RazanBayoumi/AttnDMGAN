# Text-to-Image Generation Based on AttnDM-GAN and DMAttn-GAN: Applications and Challenges
This project page provides pytorch code that implements the following papers:

Title: "Text-to-Image Generation Based on AttnDM-GAN and DMAttn-GAN: Applications and Challenges"

Link: "TO BE UPDATED SOON"

### How to use
#### Python
*	 Python 3
	
## Data
#### Birds
1. Download [metadata for birds](https://drive.google.com/file/d/1O_LtUP9sch09QH3s_EBAgLEctBQ5JBSJ/view?usp=sharing) and extract them to data/
    - `python google_drive.py 1O_LtUP9sch09QH3s_EBAgLEctBQ5JBSJ ../data/bird.zip`
    - `unzip bird.zip`
 
2. Download the [birds](https://drive.google.com/file/d/1hbzc_P1FuxMkcabkgn9ZKinBwW683j45/view?usp=sharing) image data. Extract them to data/birds/ 
    - `python google_drive.py 1hbzc_P1FuxMkcabkgn9ZKinBwW683j45 ../bird.zip`
    - `tar -xvzf CUB_200_2011.tgz`
 
#### Faces
* Download [metadata for CelebAText faces](https://drive.google.com/file/d/16m-eR9W8dm0-T21igA1dwVq0fAZwnnGX/view?usp=sharing) and extract them to data/faces/

    - `python google_drive.py 1ao16xGvVmBltWadn21fIpxk2NGytEBLg ../data/faces.zip`
  
* Download [metadata for CelebAText-HQ faces](https://drive.google.com/file/d/1V6PGK4aY7AkEVuYUR-lhdP3u3RLQhraz/view?usp=sharing) and extract them to data/faces/

    - `python google_drive.py 1V6PGK4aY7AkEVuYUR-lhdP3u3RLQhraz ../data/faces.zip`

## Pretrained Models
* [DAMSM for birds](https://drive.google.com/file/d/1GNUKjVeyWYBJ8hEU-yrfYQpDOkxEyP3V/view?usp=sharing) : Download and extract it to DAMSMencoders/
    - `python google_drive.py 1GNUKjVeyWYBJ8hEU-yrfYQpDOkxEyP3V ../DAMSMencoders/bird.zip`

* [DAMSM for CelebAText dataset](https://drive.google.com/file/d/1ibwy7-sZ2xVi5Qp_hZsic1TjmIjRmMwX/view?usp=sharing) : Download and extract it to DAMSMencoders/
    - `python google_drive.py 1ao16xGvVmBltWadn21fIpxk2NGytEBLg DAMSMencoders/faces.zip`

* [DAMSM for CelebAText-HQ dataset](https://drive.google.com/file/d/1isI_eXHrRIkhyNbzZpJDSq-rhCno58-n/view?usp=sharing) : Download and extract it to DAMSMencoders/
    - `python google_drive.py 1isI_eXHrRIkhyNbzZpJDSq-rhCno58-n DAMSMencoders/faces.zip`

## Training
#### Birds
	1- go into code/folder
	2- python main.py --cfg cfg/birds_DMGAN.yml --gpu 0
  
#### Faces
	1- go into code/folder
	2- python main.py --cfg cfg/faces_DMGAN.yml --gpu 0

## Validation
#### Birds
	- Image Generation
		1- go into code/ folder
		2- python main.py --cfg cfg/eval_birds.yml --gpu 0
    
#### Faces
	- Image Generation
		1- go into code/ folder
		2- python main.py --cfg cfg/eval_birds.yml --gpu 0
