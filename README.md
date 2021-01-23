# env-mac

1.デスクトップの「jupyter_env」ディレクトリにDockerfileを入れておく

2.以下のコマンドを実行

~/Desktop/python_env

docker build --platform linux/amd64 .

=>Successfully built d723190a8650

docker run -p 8888:8888 -v ~/Desktop/jupyter_env:/work --name my-lab d723190a8650
