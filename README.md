# EMNIST-Letters

- demo page
https://mbotsu.github.io/emnist-letters/

## Convert
$ tensorflowjs_converter --input_format keras mnist_cnn_model.h5 model_fp16 --quantize_float16

## ENV

```
% python3 -m venv env
% source env/bin/activate
(env) % pip install tensorflow-cpu tensorflow_datasets
(env) % pip install jupyter
(env) % pip install numpy emnist

tensorflowjsは、jupyterの依存エラー起きるので別の環境でセットアップ

% python3 -m venv tfjsenv
% source tfjsenv/bin/activate
(tfjsenv) % pip install tensorflowjs
(tfjsenv) % tensorflowjs_converter --input_format keras mnist_cnn_model.h5 model
```

# References
- https://dida.do/blog/how-to-deploy-a-tensorflow-model-as-a-javascript-web-app
- https://github.com/dida-do/public/blob/master/handwriting_app/EMNISTKeras.ipynb
