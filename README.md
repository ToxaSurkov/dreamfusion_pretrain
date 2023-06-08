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
