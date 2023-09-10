# AMR



Script to map single ENG sentence to DAIDE:

Download the pre-trained model file from:

https://drive.google.com/file/d/1Snne-h_vaO8WcCVGqk4PZRuGacSDyMif/view?usp=drive_link

and put the model under personal/SEN_REC_MODEL/

<details>
<summary>CLI examples</summary>

```
python single.py --english "I propose ally between us" --sender "Russia" --recipient "Turkey"
``` 
</details>

If you have a test file containing several AMRs, please refer to DAIDE/Diplomacy/README.md to parse it from AMR to DAIDE.

You can also train and test your own dataset of sentences and AMRs using the code below

make sure your dataset should under 

AMR/amrlib/amrlib/data/diplomacy/training/

AMR/amrlib/amrlib/data/diplomacy/dev/

AMR/amrlib/amrlib/data/diplomacy/test/

<details>
<summary>CLI examples_2</summary>

```
cd AMR/amrlib/scripts/33_Model_Parse_XFM
python 10_Collect_AMR_Data.py
python 20_Train_Model.py
python 22_Test_Model.py
``` 
</details>

Current Loaded Modules on CARC:
1) gcc/11.3.0   2) openblas/0.3.21   3) openmpi/4.1.4   4) pmix/3.2.3   5) usc/11.3.0 