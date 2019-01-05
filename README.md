# pytorch_tutorial

# 環境構築
dockerを使う
- docker-for-macのインストール
- `docker run -it -p 8888:8888 -v ${PWD}/src:/root/sharedfolder --ipc=host ufoym/deepo:all-py36-jupyter jupyter notebook --no-browser --ip=0.0.0.0 --allow-root --NotebookApp.token= --notebook-dir='/root'`
  - see: https://github.com/ufoym/deepo
colabでもいい
- https://colab.research.google.com/notebooks/welcome.ipynb?hl=ja
