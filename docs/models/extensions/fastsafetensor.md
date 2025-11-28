Loading Model weights with fastsafetensors
===================================================================

Using fastsafetensors library enables loading model weights to GPU memory by leveraging GPU direct storage. See [their GitHub repository](https://github.com/foundation-model-stack/fastsafetensors) for more details.

To enable this feature, you first need to install `fastsafetensors`:

```bash
pip install vllm[fastsafetensors]
```

Then, use the `--load-format fastsafetensors` command-line argument:

```bash
vllm serve facebook/opt-125m --load-format fastsafetensors
```
