# dreamfusion_pretrain

download latest DreamFusion Docker: 
``` bash
docker pull toxasurkov/full
```

get ready for pre-train (in docker):
``` bash
cd stable-dreamfusion
git pull https://github.com/ToxaSurkov/dreamfusion_pretrain.git
cp -R dreamfusion_pretrain/. .
```

pretrain:
put your fox-like (https://github.com/NVlabs/instant-ngp/tree/master/data/nerf/fox) data in /stable-dreamfusion/data/
``` bash
python3 main_pretrain --text "None" --workspace trial -O 
```

to repeat dreambooth experiments train you dreambooth model (https://dreambooth.github.io/) or download our pre-trained model (https://drive.google.com/file/d/18baFHo--GlOWRX0VLmlnFeBAmLxQHmNv/view?usp=sharing)
```bash 
cd stable-dreamfsion
python3 main --text "sks car" --hf_key path_to_model/model_name --workspace trial -O
```
