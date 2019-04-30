# Create IR Model
## Learning MNIST and Create ONNX Model

~~~python
python3 mnist.py
~~~

## Convert ONNX Model to IR Model

```
cd C:\Program Files (x86)\IntelSWTools\openvino_2019.1.087\deployment_tools\model_optimizer\install_prerequisites
install_prerequisites_onnx.bat
python3 mo.py --input_model mnist.onnx --output_dir C:\Work\
```

# Inference

## src
See main.cpp.

## Infer
infer.exe CPU C:\Work\mnist.xml "C:\Work\one.png"
