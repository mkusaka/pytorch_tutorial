# pytorch_tutorial

# 環境構築
dockerを使う
- docker-for-macのインストール
- deepoのimageをビルドして起動

```bash
git clone https://github.com/ufoym/deepo.git
docker build . -f deepo/docker/Dockerfile.all-jupyter-py36-cpu -t deepo/all:cpu
docker run --rm -it -p 8888:8888 -v ${PWD}/src:/root/sharedfolder --ipc=host deepo/all:cpu jupyter notebook --no-browser --ip=0.0.0.0 --allow-root --NotebookApp.token= --notebook-dir='/root'
```
  - see: https://github.com/ufoym/deepo

- colabでもいい
  - https://colab.research.google.com/notebooks/welcome.ipynb?hl=ja

# ソース
- pytorchのtutorialとか
  - [強化学習](https://pytorch.org/tutorials/intermediate/reinforcement_q_learning.html)
