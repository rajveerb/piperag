## Kepler2

conda create -n retro python=3.9 -y
conda activate retro
pip3 install torch==2.1.0 torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
pip install transformers==4.21.0 
pip install pip==23.3.2
pip install pytorch-lightning==1.7.4 
pip install einops==0.6.0 
pip install pytest==7.2.1 
pip install sentence-transformers==2.2.2 
pip install matplotlib==3.6.3  
pip install seaborn==0.12.2
pip install torchmetrics==0.11.4
pip install onnx==1.15
pip install onnxruntime-gpu==1.16
pip install grpcio-tools
conda install -c pytorch -c nvidia faiss-gpu=1.7.4 mkl=2021 blas=1.0=mkl
# Below needs to be added due to https://github.com/easydiffusion/easydiffusion/issues/1851 error
pip install huggingface-hub==0.25.2
export WORKSPACE=$PWD