This is project for the neural machine translation system from Quechua to Spanish.
The code and corpora is part of a paper authored by John E. Ortega (NYU), Richard Castro Mamani (Cuzco) , and Kyunghun Cho (NYU)

The annotations folder are the human subject evaluations and the corpora are the new corpora commissioned by us @NYU, specifically the "magazine" folder under corpora has 100 translations done by a professional Quechua->Spanish translator.

The Opus folder contains files gotten using jw300 on http://opus.nlpl.eu/

There is a train,validate,test split for training OpenNmt (or any MT) models...

### PRE-TRAINED & TRAINED MODELS

###### opus_jw_300

```
wget --max-redirect=20 -O opus_jw_300.zip https://www.dropbox.com/sh/a0la2qd23fh0e67/AADxks2LdWbyRwxp9lXREE50a?dl=0

unzip opus_jw_300.zip

onmt_translate -model train_bpe_europarl_and_jw300_joint_qu_es_es_qu-model_step_20000.pt -src /home/ubuntu/mt_quechua_spanish/corpora/magazine/kallpa.qu.truecase -output kallpa

```

