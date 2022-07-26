Reference: [NVIDIA/tacotron2](https://github.com/NVIDIA/tacotron2)

## How to use
1. Put raw Japanese texts in ./filelists
2. Put WAV files in ./wav
3. (Optional) Download NVIDIA's [pretrained model](https://drive.google.com/file/d/1c5ZTuT7J08wLUoVZ2KkUs_VdZuJ86ZqA/view?usp=sharing)
4. Open ./train.ipynb to install requirements and start training
5. Download NVIDIA's [WaveGlow model](https://drive.google.com/open?id=1rpK8CzAAirq9sWZhe9nlfvxMF1dRgFbF)
6. Open ./inference.ipynb to generate voice

## Cleaners
File ./hparams.py line 30
1. 'japanese_cleaners'
before: 何かあったらいつでも話して下さい。学院のことじゃなく、私事に関することでも何でも
after: nanikaacltaraitsudemohanashItekudasai.gakuiNnokotojanaku,shijinikaNsurukotodemonanidemo.
2. 'japanese_tokenization_cleaners'
before: 何かあったらいつでも話して下さい。学院のことじゃなく、私事に関することでも何でも
after: nani ka acl tara itsu demo hanashi te kudasai. gakuiN no koto ja naku, shiji nikaNsuru koto de mo naNdemo.

